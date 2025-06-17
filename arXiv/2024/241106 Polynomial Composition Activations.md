https://arxiv.org/abs/2411.03884

*Polynomial Composition Activations: Unleashing the Dynamics of Large Language Models* (Zhijian Zhuo, Ya Wang, Yutao Zeng, Xiaoqing Li, Xun Zhou, Jinwen Ma)

> Transformers have found extensive applications across various domains due to the powerful fitting capabilities. This success can be partially attributed to their inherent nonlinearity. Thus, in addition to the ReLU function employed in the original transformer architecture, researchers have explored alternative modules such as GeLU and SwishGLU to enhance nonlinearity and thereby augment representational capacity. In this paper, we propose a novel category of polynomial composition activations (PolyCom), designed to optimize the dynamics of transformers. Theoretically, we provide a comprehensive mathematical analysis of PolyCom, highlighting its enhanced expressivity and efficacy relative to other activation functions. Notably, we demonstrate that networks incorporating PolyCom achieve the $\textbf{optimal approximation rate}$, indicating that PolyCom networks require minimal parameters to approximate general smooth functions in Sobolev spaces. We conduct empirical experiments on the pre-training configurations of large language models (LLMs), including both dense and sparse architectures. By substituting conventional activation functions with PolyCom, we enable LLMs to capture higher-order interactions within the data, thus improving performance metrics in terms of accuracy and convergence rates. Extensive experimental results demonstrate the effectiveness of our method, showing substantial improvements over other activation functions. Code is available at https://github.com/BryceZhuo/PolyCom.

비선형 함수의 다항식으로 구성한 Activation 함수. Activation과 Optimizer는 건드리지 말라는 것이 딥 러닝 판의 오랜 격언이긴 했습니다만...SwiGLU 같은 Activation도 절찬리에 사용되고 있다는 것을 고려하면 속도에 큰 손해가 없으면 쓸 수도 있겠다 싶긴 합니다.

<english>
Activation function that consist of polynomial of nonlinear functions. It is old wisdom in the field of deep learning that it is better not to deal with activation and optimizers, but as nowadays activations like SwiGLU is commonly used, maybe we can use more exotic activations if it is not slow too much.
</english>

#activation #transformer 