https://arxiv.org/abs/2404.14507

*Align Your Steps: Optimizing Sampling Schedules in Diffusion Models* (Amirmojtaba Sabour, Sanja Fidler, Karsten Kreis)

> Diffusion models (DMs) have established themselves as the state-of-the-art generative modeling approach in the visual domain and beyond. A crucial drawback of DMs is their slow sampling speed, relying on many sequential function evaluations through large neural networks. Sampling from DMs can be seen as solving a differential equation through a discretized set of noise levels known as the sampling schedule. While past works primarily focused on deriving efficient solvers, little attention has been given to finding optimal sampling schedules, and the entire literature relies on hand-crafted heuristics. In this work, for the first time, we propose a general and principled approach to optimizing the sampling schedules of DMs for high-quality outputs, called $\textit{Align Your Steps}$. We leverage methods from stochastic calculus and find optimal schedules specific to different solvers, trained DMs and datasets. We evaluate our novel approach on several image, video as well as 2D toy data synthesis benchmarks, using a variety of different samplers, and observe that our optimized schedules outperform previous hand-crafted schedules in almost all experiments. Our method demonstrates the untapped potential of sampling schedule optimization, especially in the few-step synthesis regime.

Diffusion 모델의 샘플링 과정에서 사용하는 SDE Solver의 Discretization에서 발생하는 에러를 최소화하기 위한 샘플링 스케줄을 유도. 갑자기 디테일 수준이 달라지는군요.

#diffusion 