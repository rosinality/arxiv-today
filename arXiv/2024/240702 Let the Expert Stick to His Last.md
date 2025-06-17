https://arxiv.org/abs/2407.01906

*Let the Expert Stick to His Last: Expert-Specialized Fine-Tuning for Sparse Architectural Large Language Models* (Zihan Wang, Deli Chen, Damai Dai, Runxin Xu, Zhuoshu Li, Y. Wu)

let> Parameter-efficient fine-tuning (PEFT) is crucial for customizing Large Language Models (LLMs) with constrained resources. Although there have been various PEFT methods for dense-architecture LLMs, PEFT for sparse-architecture LLMs is still underexplored. In this work, we study the PEFT method for LLMs with the Mixture-of-Experts (MoE) architecture and the contents of this work are mainly threefold: (1) We investigate the dispersion degree of the activated experts in customized tasks, and found that the routing distribution for a specific task tends to be highly concentrated, while the distribution of activated experts varies significantly across different tasks. (2) We propose Expert-Specialized Fine-Tuning, or ESFT, which tunes the experts most relevant to downstream tasks while freezing the other experts and modules; experimental results demonstrate that our method not only improves the tuning efficiency, but also matches or even surpasses the performance of full-parameter fine-tuning. (3) We further analyze the impact of the MoE architecture on expert-specialized fine-tuning. We find that MoE models with finer-grained experts are more advantageous in selecting the combination of experts that are most relevant to downstream tasks, thereby enhancing both the training efficiency and effectiveness.

MoE 모델의 Expert Activation이 각각 특정한 과제에 집중되어 있다는 것을 발견. 과제에 대해 Activate 되는 Expert를 골라 그 Expert만 학습시키는 것으로 PEFT를 할 수 있다는 아이디어. 공유 Expert가 있고 작은 Expert를 여러 개 사용하는 DeepSeek 스타일의 MoE의 특성일 수도 있을 것 같습니다. (Mixtral 같은 경우 Expert가 서로 유사하죠. https://arxiv.org/abs/2406.18219)

#moe #efficient-training #multitask

# Links

[[240626 A Closer Look into Mixture-of-Experts in Large Language Models.md]]