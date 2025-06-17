https://arxiv.org/abs/2505.02831

*No Other Representation Component Is Needed: Diffusion Transformers Can Provide Representation Guidance by Themselves* (Dengyang Jiang, Mengmeng Wang, Liuzhuozheng Li, Lei Zhang, Haoyu Wang, Wei Wei, Guang Dai, Yanning Zhang, Jingdong Wang)

> Recent studies have demonstrated that learning a meaningful internal representation can both accelerate generative training and enhance generation quality of the diffusion transformers. However, existing approaches necessitate to either introduce an additional and complex representation training framework or rely on a large-scale, pre-trained representation foundation model to provide representation guidance during the original generative training process. In this study, we posit that the unique discriminative process inherent to diffusion transformers enables them to offer such guidance without requiring external representation components. We therefore propose Self-Representation A}lignment (SRA), a simple yet straightforward method that obtain representation guidance through a self-distillation manner. Specifically, SRA aligns the output latent representation of the diffusion transformer in earlier layer with higher noise to that in later layer with lower noise to progressively enhance the overall representation learning during only generative training process. Experimental results indicate that applying SRA to DiTs and SiTs yields consistent performance improvements. Moreover, SRA not only significantly outperforms approaches relying on auxiliary, complex representation training frameworks but also achieves performance comparable to methods that heavily dependent on powerful external representation priors.

Diffusion 모델 학습에 DINOv2 같은 외부 모델 대신 Diffusion 모델의 EMA로 가이드를 줄 수 있다는 아이디어군요.

<english>
The idead that instead of external models like DINOv2 it is possible to EMA of diffusion models to guide the training of diffusion models.
</english>

#diffusion 