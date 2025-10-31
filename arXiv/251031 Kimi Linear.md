https://github.com/MoonshotAI/Kimi-Linear/blob/master/tech_report.pdf

*Kimi Linear: An Expressive, Efficient Attention Architecture* (Kimi Team)

> We introduce Kimi Linear, a hybrid linear attention architecture that, for the first time, outperforms full attention under fair comparisons across various scenarios—including short-context, long-context, and reinforcement learning (RL) scaling regimes. At its core lies Kimi Delta Attention (KDA), an expressive linear attention module that extends Gated DeltaNet [111] with a finer-grained gating mechanism, enabling more effective use of limited finite-state RNN memory. Our bespoke chunkwise algorithm achieves high hardware efficiency through a specialized variant of the Diagonal-Plus-Low- Rank (DPLR) transition matrices, which substantially reduces computation compared to the general DPLR formulation while remaining more consistent with the classical delta rule. We pretrain a Kimi Linear model with 3B activated parameters and 48B total parameters, based on a layerwise hybrid of KDA and Multi-Head Latent Attention (MLA). Our experiments show that with an identical training recipe, Kimi Linear outperforms full MLA with a sizeable margin across all evaluated tasks, while reducing KV cache usage by up to 75% and achieving up to 6× decoding throughput for a 1M context. These results demonstrate that Kimi Linear can be a drop-in replacement for full attention architectures with superior performance and efficiency, including tasks with longer input and output lengths. To support further research, we open-source the KDA kernel and vLLM implementations 1, and release the pre-trained and instruction-tuned model checkpoints. 

Gated DeltaNet + Fine grained gating. Global Attention에는 NoPE를 사용. 순수 어텐션을 추론에서 상회. SSM 하이브리드가 바닐라에 비해 서로 다른 Inductive Bias로 인해 더 나은 성능을 나타낼 수 있는 가능성은 아주 흥미로운 방향이라고 생각.

NoPE에 대해서 Long Context에서 위치를 포착하는 능력을 잃게 될 우려가 있다고 생각하고 있었는데 KDA가 Global Attention에서 RoPE가 적용되지 않은 것을 보완할 수 있다는 것도 흥미로운 지점.

Test Time Training은 시퀀스 모델에 대한 분석에 유용한 프레임워크. Gated Linear Attention인 Mamba와 DeltaNet의 차이를 대조하는 한 가지 방법은 Full 배치 GD와 미니 배치 GD의 차이로 생각하는 것. https://arxiv.org/abs/2407.04620, https://arxiv.org/abs/2501.12352

한 가지 더 - 표준적인 벤치마크들은 이제 아키텍처의 성능, 특히 추론에 대한 성능을 평가하는데 충분하지 않음. 이 부분에 대해 아주 철저할 필요가 있음. https://arxiv.org/abs/2510.24397

Gated DeltaNet + fine grained gating, and NoPE for global attention. Outperforms pure attention in reasoning. I think what is really interesting about SSM is it can actually be better than vanilla due to different inductive bias.

What made me worry about NoPE is it may lose the ability to localize in long contexts. KDA shows maybe it can compensate for the lack of RoPE in global attention.

Test time training is a nice framework to think about sequence models. One interesting way to contrast gated linear attention like Mamba vs DeltaNet is full-batch GD vs mini-batch GD. https://arxiv.org/abs/2407.04620, https://arxiv.org/abs/2501.12352

One more point - standard benchmarks are not enough to verify effectiveness of architectures, especially on reasoning tasks. We need to be very thorough on this. https://arxiv.org/abs/2510.24397

#efficient-attention #state-space-model 