https://arxiv.org/abs/2410.16794

*One-Step Diffusion Distillation through Score Implicit Matching* (Weijian Luo, Zemin Huang, Zhengyang Geng, J. Zico Kolter, Guo-jun Qi)

> Despite their strong performances on many generative tasks, diffusion models require a large number of sampling steps in order to generate realistic samples. This has motivated the community to develop effective methods to distill pre-trained diffusion models into more efficient models, but these methods still typically require few-step inference or perform substantially worse than the underlying model. In this paper, we present Score Implicit Matching (SIM) a new approach to distilling pre-trained diffusion models into single-step generator models, while maintaining almost the same sample generation ability as the original model as well as being data-free with no need of training samples for distillation. The method rests upon the fact that, although the traditional score-based loss is intractable to minimize for generator models, under certain conditions we can efficiently compute the gradients for a wide class of score-based divergences between a diffusion model and a generator. SIM shows strong empirical performances for one-step generators: on the CIFAR10 dataset, it achieves an FID of 2.06 for unconditional generation and 1.96 for class-conditional generation. Moreover, by applying SIM to a leading transformer-based diffusion model, we distill a single-step generator for text-to-image (T2I) generation that attains an aesthetic score of 6.42 with no performance decline over the original multi-step counterpart, clearly outperforming the other one-step generators including SDXL-TURBO of 5.33, SDXL-LIGHTNING of 5.34 and HYPER-SDXL of 5.85. We will release this industry-ready one-step transformer-based T2I generator along with this paper.

1 step Generator에 대한 Diffusion Distillation. 이미지 생성 자체를 목표로 한다면 Autoregressive 모델은 Distill된 Diffusion 모델과 경쟁해야 하겠죠.

<english>
Diffusion distillation for 1 step generator. If we intend to image generation, autoregressive models should compete with distilled diffusion models.
</english>

#distillation #diffusion 