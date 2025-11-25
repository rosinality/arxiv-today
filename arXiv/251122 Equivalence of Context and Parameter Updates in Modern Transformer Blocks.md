https://arxiv.org/abs/2511.17864

*Equivalence of Context and Parameter Updates in Modern Transformer Blocks* (Adrian Goldwaser, Michael Munn, Javier Gonzalvo, Benoit Dherin)

> Recent research has established that the impact of context in a vanilla transformer can be represented implicitly by forming a token-dependent, rank-1 patch to its MLP weights. This work extends that foundational theory to the diverse architectures of modern Large Language Models. We first demonstrate a precise, analytical solution for a Gemma-style transformer block, proving that the entire effect of a context can be perfectly mapped to rank-1 patches on its MLP weight matrices and a patch to the RMSNorm scale. We then generalize this result, providing a constructive proof and algorithm for multi-layer models. To unify these findings, we introduce a general framework centered on two core properties: input controllability and output controllability. We prove that a perfect implicit weight patch is possible for any MLP block where the inner function is input-controllable and the outer function is output-controllable. This provides a simpler and more powerful lens for understanding how transformer models transmute prompts into effective weights. This setup generalizes to a wide range of modern LLM architectures including gating, pre-/post-norm, mixture of experts and sequential/parallel transformer blocks.

컨텍스트 입력이 어떻게 FFN에 대한 랭크 1 업데이트로 흡수될 수 있는가에 대한 분석. 일반적으로 x + g(f(x)) 형태의 ResNet이면서 입력이 f의 Weight로 흡수될 수 있고 출력이 g의 Weight로 흡수될 수 있다면 이러한 특성을 갖게됨.

반대로 컨텍스트 입력에 의한 영향은 FFN에 대한 랭크 1 업데이트 이상이 될 수 없다는 것을 의미할지도?

Analysis of how context can be absorbed as a rank 1 update to FFN. In general a resnet in the form of x + g(f(x)) with f allowing input to be absorbed into weights, and g allowing output to be absorbed into weights enables this property.

Conversely maybe this implies contextual modification cannot go further than rank 1 update to FFN.

#transformer 