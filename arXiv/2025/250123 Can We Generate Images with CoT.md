https://arxiv.org/abs/2501.13926

*Can We Generate Images with CoT? Let's Verify and Reinforce Image Generation Step by Step* (Ziyu Guo, Renrui Zhang, Chengzhuo Tong, Zhizheng Zhao, Peng Gao, Hongsheng Li, Pheng-Ann Heng)

> Chain-of-Thought (CoT) reasoning has been extensively explored in large models to tackle complex understanding tasks. However, it still remains an open question whether such strategies can be applied to verifying and reinforcing image generation scenarios. In this paper, we provide the first comprehensive investigation of the potential of CoT reasoning to enhance autoregressive image generation. We focus on three techniques: scaling test-time computation for verification, aligning model preferences with Direct Preference Optimization (DPO), and integrating these techniques for complementary effects. Our results demonstrate that these approaches can be effectively adapted and combined to significantly improve image generation performance. Furthermore, given the pivotal role of reward models in our findings, we propose the Potential Assessment Reward Model (PARM) and PARM++, specialized for autoregressive image generation. PARM adaptively assesses each generation step through a potential assessment approach, merging the strengths of existing reward models, and PARM++ further introduces a reflection mechanism to self-correct the generated unsatisfactory image. Using our investigated reasoning strategies, we enhance a baseline model, Show-o, to achieve superior results, with a significant +24% improvement on the GenEval benchmark, surpassing Stable Diffusion 3 by +15%. We hope our study provides unique insights and paves a new path for integrating CoT reasoning with autoregressive image generation. Code and models are released at https://github.com/ZiyuGuo99/Image-Generation-CoT

Autoregressive Image Generation에서 생성 과정 중에 Reward Model을 통한 탐색이 가능한가에 대한 연구. Diffusion의 Inference Time Scaling (https://arxiv.org/abs/2501.09732) 연구와 비슷한 점이 있습니다. 여기서는 Masked Token Prediction을 사용하기에 생성 초반에도 Process Reward를 적용할 수 있는지 테스트했는데 아무래도 초기에는 이미지 상태가 좋지 않으니 이점이 없었다고 하네요. 이를 위한 방법을 설계했습니다.

<english>
A study on whether it is possible to search using reward model during generation process of autoregressive image model. It is similar vein of research with inference time scaling for diffusion (https://arxiv.org/abs/2501.09732). As this study used makekd token prediction models they tested whether process reward can be applied, but they reports it does not work well due to low image quality of early generated images. They designed a method for this.
</english>

#inference-time-scaling #reward-model #autoregressive-model

# Links

[[250116 Inference-Time Scaling for Diffusion Models beyond Scaling Denoising Steps.md]]