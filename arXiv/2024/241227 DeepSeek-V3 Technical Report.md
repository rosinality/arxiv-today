https://github.com/deepseek-ai/DeepSeek-V3/blob/main/DeepSeek_V3.pdf

*DeepSeek-V3 Technical Report* (DeepSeek-AI)

> We present DeepSeek-V3, a strong Mixture-of-Experts (MoE) language model with 671B total parameters with 37B activated for each token. To achieve efficient inference and cost-effective training, DeepSeek-V3 adopts Multi-head Latent Attention (MLA) and DeepSeekMoE architec- tures, which were thoroughly validated in DeepSeek-V2. Furthermore, DeepSeek-V3 pioneers an auxiliary-loss-free strategy for load balancing and sets a multi-token prediction training objective for stronger performance. We pre-train DeepSeek-V3 on 14.8 trillion diverse and high-quality tokens, followed by Supervised Fine-Tuning and Reinforcement Learning stages to fully harness its capabilities. Comprehensive evaluations reveal that DeepSeek-V3 outperforms other open-source models and achieves performance comparable to leading closed-source models. Despite its excellent performance, DeepSeek-V3 requires only 2.788M H800 GPU hours for its full training. In addition, its training process is remarkably stable. Throughout the entire training process, we did not experience any irrecoverable loss spikes or perform any rollbacks. The model checkpoints are available at https://github.com/deepseek-ai/DeepSeek-V3.

37B Activated 671B Total Weight MoE, 14.8T 학습 모델. H800 2048개만으로 3.5 Sonnet 수준의 벤치마크 스코어를 달성했습니다. (R1 Distill 덕인지 수학 스코어는 더 우수하네요.)

DeepSeek-V2와 기본적으로는 비슷한 구조입니다. 다만 Aux-Loss-Free Load Balancing에 (https://arxiv.org/abs/2408.15664) 추가적으로 Sequence-level Aux Loss를 사용하고 Token Dropping을 제거했군요. 거기에 Multi Token Prediction을 (https://arxiv.org/abs/2404.19737) 사용했네요. Sequence Packing 개선도 있습니다. (https://arxiv.org/abs/2404.10830)

학습 인프라와 관련해서는 Zero Bubble Pipeline Parallel을 (https://arxiv.org/abs/2401.10241) 자신들이 개발한 DualPipe 스케줄로 바꿨군요. All-to-All 커널을 최적화하면서 Communication에 사용할 GPU SM을 직접 할당해 관리하는 형태를 사용했습니다.

그리고 FP8 학습을 했군요. Group Quantization을 했고 FP32로 연산 결과를 누적하는 방법을 사용했습니다. Microscaling 포맷을 미리 썼다는 느낌이군요. 아예 Attention 바로 뒤의 Linear 연산 같이 민감한 영역은 E5M6 포맷을 새로 만들어서 썼습니다.

추론에서는 프리필과 디코드에 배포된 모델이 구분되어 있습니다. 프리필에서는 TP4, DP8, EP32로 4 노드 32 GPU 단위이고 디코드에는 TP4, DP80, EP320으로 40 노드 320 GPU 단위네요.

이 과정에서 작업이 많았기 때문인지 SM 없이 통신을 할 수 있도록 하고 (https://discuss.pytorch.org/t/distributed-w-torchtitan-introducing-async-tensor-parallelism-in-pytorch), InfiniBand와 NVLink에 대한 통합 인터페이스, 고정밀도 Accumulation, Group Quantization, Online Quantization, Transposed GEMM이 나왔으면 좋겠다는 이야기를 따로 썼네요.

포스트트레이닝에서는 DeepSeek-R1을 사용한 추론 데이터가 들어가기 시작했네요. 코드나 수학 같은 영역에 대한 전문 모델을 R1 데이터를 기반으로 구축해서 이 모델로부터 SFT 데이터를 생성하는 방법을 사용했습니다. Reward Model로는 컴파일러 피드백 같은 규칙 기반 RM에 더해 Reward에 대한 Chain of Thought도 사용했군요. 여기에 Constitutional AI 스타일의 Self Alignment도 들어갔네요. 그리고 GRPO를 여전히 사용했습니다.

DeepSeek 창립자가 인터뷰에서 Llama 스타일의 아키텍처와 현재 알려진 학습 방법은 연산 효율성 측면에서 프런티어 레벨에 크게 밀린다는 이야기를 한 적이 있습니다. (https://www.chinatalk.media/p/deepseek-ceo-interview-with-chinas) 그게 사실이라는 것을 직접 증명했네요.

<english>
MoE with 32B activated and 671B total weight, trained on 14.8T. They reached 3.5 Sonnet level benchmark with only 2048 H800s. (Actually, they surpass it on math benchmark due to R1 distillation.)

Basically it is similar architecture with DeepSeek-V2. But they used auxiliary-loss-free load balancing (https://arxiv.org/abs/2408.15664), in addition to sequence level auxiliary loss, without token dropping. They used multi token prediction (https://arxiv.org/abs/2404.19737). Also, they improved sequence packing ( (https://arxiv.org/abs/2404.10830).

For training infrastructure they changed Zero-Bubble Pipeline Parallel to their own DualPipe schedule. For optimizing all-to-all kernels they manually allocated and managed GPU SM for communication.

And then they used FP8 training. They used group quantization and full precision accumulation. It will be similar to microscaling format that introduced in Blackwell. For sensitive activations like linear after attention they used custom E5M6 format.

In inference they used separate deployment setup for prefill and decode. For prefill they used TP4, DP8, EP32 on 4 node and 32 GPU as a single deployment unit. For decode they used TP4, DP80, EP320 on 40 node and 320 GPU as a unit.

And it seems that this kind of optimizations required them a lot of work. So they wrote separately suggesting to hardware vendor to implement communication without SM (https://discuss.pytorch.org/t/distributed-w-torchtitan-introducing-async-tensor-parallelism-in-pytorch), an unified interface for InfiniBand and NVLink, full precision accumulation, group quantization, online quantization, transposed GEMM.

In post-training they started to use reasoning data using DeepSeek-R1. They trained expert models for domains like math and code using the data generated from R1, and generated SFT data by doing rejection sampling on it. For reward models they used rule based RM like compiler feedback, and reward with chain of thought. Also they used self alignment in style of Constitutional AI. And they still uses GRPO.

Founder of DeepSeek once said in the interview that Llama styled architecture and currently known method for training is far behind the frontier level (https://www.chinatalk.media/p/deepseek-ceo-interview-with-chinas). They proved it is true by their own.
</english>

#llm #reasoning #post-training #efficient-training #quantization #moe 