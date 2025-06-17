https://arxiv.org/abs/2410.12557

*One Step Diffusion via Shortcut Models* (Kevin Frans, Danijar Hafner, Sergey Levine, Pieter Abbeel)

> Diffusion models and flow-matching models have enabled generating diverse and realistic images by learning to transfer noise to data. However, sampling from these models involves iterative denoising over many neural network passes, making generation slow and expensive. Previous approaches for speeding up sampling require complex training regimes, such as multiple training phases, multiple networks, or fragile scheduling. We introduce shortcut models, a family of generative models that use a single network and training phase to produce high-quality samples in a single or multiple sampling steps. Shortcut models condition the network not only on the current noise level but also on the desired step size, allowing the model to skip ahead in the generation process. Across a wide range of sampling step budgets, shortcut models consistently produce higher quality samples than previous approaches, such as consistency models and reflow. Compared to distillation, shortcut models reduce complexity to a single network and training phase and additionally allow varying step budgets at inference time.

가변 샘플링 스텝에 대응 가능한 단순한 방법이군요. 스텝 크기를 모델의 입력으로 주는데, 스텝 두 번이 2배 크기의 스텝과 같아야 한다는 Self Distillation 형태의 Objective를 사용합니다.

<english>
Simple approach for supporting variable sampling steps. Step size is used as a model input, and uses self distillation like objectives that two steps should be similar to one step with twice step sizes.
</english>

#diffusion 