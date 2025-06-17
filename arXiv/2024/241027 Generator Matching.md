https://arxiv.org/abs/2410.20587

*Generator Matching: Generative modeling with arbitrary Markov processes* (Peter Holderrieth, Marton Havasi, Jason Yim, Neta Shaul, Itai Gat, Tommi Jaakkola, Brian Karrer, Ricky T. Q. Chen, Yaron Lipman)

> We introduce generator matching, a modality-agnostic framework for generative modeling using arbitrary Markov processes. Generators characterize the infinitesimal evolution of a Markov process, which we leverage for generative modeling in a similar vein to flow matching: we construct conditional generators which generate single data points, then learn to approximate the marginal generator which generates the full data distribution. We show that generator matching unifies various generative modeling methods, including diffusion models, flow matching and discrete diffusion models. Furthermore, it provides the foundation to expand the design space to new and unexplored Markov processes such as jump processes. Finally, generator matching enables the construction of superpositions of Markov generative processes and enables the construction of multimodal models in a rigorous manner. We empirically validate our method on protein and image structure generation, showing that superposition with a jump process improves image generation.

임의 마르코프 과정에 대한 생성 모형. 따라서 Flow Matching이나 Diffusion 같은 Objective를 통합하는 방법입니다. 추가로 임의 마르코프 과정이니 점프 과정 같은 확률 과정을 도입할 수 있죠.

<english>
Generative model using arbitrary markov processes. So it unifies objectives like flow matching or diffusion. Additionally as it is allowed to use arbitrary markov process, it is possible to use stochastic processes like jump process.
</english>

#generative-model #diffusion 