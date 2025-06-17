https://arxiv.org/abs/2405.18407

*Phased Consistency Model* (Fu-Yun Wang, Zhaoyang Huang, Alexander William Bergman, Dazhong Shen, Peng Gao, Michael Lingelbach, Keqiang Sun, Weikang Bian, Guanglu Song, Yu Liu, Hongsheng Li, Xiaogang Wang)

> The consistency model (CM) has recently made significant progress in accelerating the generation of diffusion models. However, its application to high-resolution, text-conditioned image generation in the latent space (a.k.a., LCM) remains unsatisfactory. In this paper, we identify three key flaws in the current design of LCM. We investigate the reasons behind these limitations and propose the Phased Consistency Model (PCM), which generalizes the design space and addresses all identified limitations. Our evaluations demonstrate that PCM significantly outperforms LCM across 1--16 step generation settings. While PCM is specifically designed for multi-step refinement, it achieves even superior or comparable 1-step generation results to previously state-of-the-art specifically designed 1-step methods. Furthermore, we show that PCM's methodology is versatile and applicable to video generation, enabling us to train the state-of-the-art few-step text-to-video generator. More details are available at https://g-u-n.github.io/projects/pcm/.

Consistency Distillation에 대한 개선. Trajectory를 쪼갠다는 점에서는 Multistep Consistency Models (https://arxiv.org/abs/2403.06807) 와 통하는 점이 있는 것 같습니다. Text Condition에 대해서 했고 Adversarial Loss를 사용했다는 점이 추가 포인트겠네요.

#diffusion

# Links

[[240311 Multistep Consistency Models.md]]