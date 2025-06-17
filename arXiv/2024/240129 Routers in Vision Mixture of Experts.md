https://arxiv.org/abs/2401.15969

*Routers in Vision Mixture of Experts: An Empirical Study* (Tianlin Liu, Mathieu Blondel, Carlos Riquelme, Joan Puigcerver)

> Mixture-of-Experts (MoE) models are a promising way to scale up model capacity without significantly increasing computational cost. A key component of MoEs is the router, which decides which subset of parameters (experts) process which feature embeddings (tokens). In this paper, we present a comprehensive study of routers in MoEs for computer vision tasks. We introduce a unified MoE formulation that subsumes different MoEs with two parametric routing tensors. This formulation covers both sparse MoE, which uses a binary or hard assignment between experts and tokens, and soft MoE, which uses a soft assignment between experts and weighted combinations of tokens. Routers for sparse MoEs can be further grouped into two variants: Token Choice, which matches experts to each token, and Expert Choice, which matches tokens to each expert. We conduct head-to-head experiments with 6 different routers, including existing routers from prior work and new ones we introduce. We show that (i) many routers originally developed for language modeling can be adapted to perform strongly in vision tasks, (ii) in sparse MoE, Expert Choice routers generally outperform Token Choice routers, and (iii) soft MoEs generally outperform sparse MoEs with a fixed compute budget. These results provide new insights regarding the crucial role of routers in vision MoE models.

비전 모델에 대한 MoE 테스트. Soft MoE가 Hard MoE 보다 낫고, 각 토큰에서 Top-K Expert를 선택하는 것보다는 각 Expert에 Top-K 토큰을 할당하는 쪽이 낫다, 그리고 그 외의 변주는 그렇게 중요하지 않은 것 같다는 결과입니다.

아키텍처적인 측면에서 MoE는 탐색할 가치가 충분히 있다고 보이네요.

#moe 

Testing MoE for vision models. It shows that Soft MoE is better than Hard MoE, and it is better to assign top-k tokens for each experts rather than selecting top-k experts for each tokens. And it also suggest that another variations for token routing and assignment is not very significant.

In architectural aspect of large models, MoE seems worth exploring.