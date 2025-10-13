https://arxiv.org/abs/2510.02300

*Equilibrium Matching: Generative Modeling with Implicit Energy-Based Models* (Runqian Wang, Yilun Du)

> We introduce Equilibrium Matching (EqM), a generative modeling framework built from an equilibrium dynamics perspective. EqM discards the non-equilibrium, time-conditional dynamics in traditional diffusion and flow-based generative models and instead learns the equilibrium gradient of an implicit energy landscape. Through this approach, we can adopt an optimization-based sampling process at inference time, where samples are obtained by gradient descent on the learned landscape with adjustable step sizes, adaptive optimizers, and adaptive compute. EqM surpasses the generation performance of diffusion/flow models empirically, achieving an FID of 1.90 on ImageNet 256$\times$256. EqM is also theoretically justified to learn and sample from the data manifold. Beyond generation, EqM is a flexible framework that naturally handles tasks including partially noised image denoising, OOD detection, and image composition. By replacing time-conditional velocities with a unified equilibrium landscape, EqM offers a tighter bridge between flow and energy-based models and a simple route to optimization-driven inference.

시간 조건을 입력으로 사용하지 않는 생성 모형. 실제 데이터에 대해서는 0으로 감소하는 그래디언트를 추정하도록 학습됨. 따라서 샘플링에 Gradient Descent를 사용할 수 있음. 흥미로움.

Time-condition-free generative model that estimates a gradient which vanishes to 0 for real samples. Thus sampling can be done using gradient descent. Interesting.

#diffusion #generative-model 