https://arxiv.org/abs/2410.14895

*Truncated Consistency Models* (Sangyun Lee, Yilun Xu, Tomas Geffner, Giulia Fanti, Karsten Kreis, Arash Vahdat, Weili Nie)

> Consistency models have recently been introduced to accelerate sampling from diffusion models by directly predicting the solution (i.e., data) of the probability flow ODE (PF ODE) from initial noise. However, the training of consistency models requires learning to map all intermediate points along PF ODE trajectories to their corresponding endpoints. This task is much more challenging than the ultimate objective of one-step generation, which only concerns the PF ODE's noise-to-data mapping. We empirically find that this training paradigm limits the one-step generation performance of consistency models. To address this issue, we generalize consistency training to the truncated time range, which allows the model to ignore denoising tasks at earlier time steps and focus its capacity on generation. We propose a new parameterization of the consistency function and a two-stage training procedure that prevents the truncated-time training from collapsing to a trivial solution. Experiments on CIFAR-10 and ImageNet $64\times64$ datasets show that our method achieves better one-step and two-step FIDs than the state-of-the-art consistency models such as iCT-deep, using more than 2$\times$ smaller networks. Project page: https://truncated-cm.github.io/

Consistency Model의 학습의 난점은 노이즈 -> 데이터라는 생성 목표와 중간 지점 -> 데이터라는 디노이징 목표가 같이 학습 되기 때문이라는 아이디어. 따라서 t를 제약해 생성 목표에 중점을 두는 것으로 성능을 개선할 수 있다는 아이디어. 다만 t를 제약하면 경계 조건이 사라져 붕괴가 일어나기 때문에 t가 제약된 상황에서 경계 조건을 설정해줍니다.

Consistency Model에 대해서는 학습 안정성에 대한 이야기가 많이 나오는군요. 무언가 GAN 시절의 추억이 떠오르고 그렇네요.

<english>
The idea that difficulties of training consistency model arose from mixed objective of generative objective that maps the noise to the data and denoising objective that maps the intermediate samples to the data. So if we improve performance by limit t and concentrating on generative objectives. But if we limit t then we lost boundary conditions and this causes model collapse. So we setup boundary conditions for situations with bounded t.

There are many papers discussing training stabilities of consistency models. It reminds me an era of GANs.
</english>

#diffusion 