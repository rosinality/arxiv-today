https://arxiv.org/abs/2412.15119

*Parallelized Autoregressive Visual Generation* (Yuqing Wang, Shuhuai Ren, Zhijie Lin, Yujin Han, Haoyuan Guo, Zhenheng Yang, Difan Zou, Jiashi Feng, Xihui Liu)

> Autoregressive models have emerged as a powerful approach for visual generation but suffer from slow inference speed due to their sequential token-by-token prediction process. In this paper, we propose a simple yet effective approach for parallelized autoregressive visual generation that improves generation efficiency while preserving the advantages of autoregressive modeling. Our key insight is that parallel generation depends on visual token dependencies-tokens with weak dependencies can be generated in parallel, while strongly dependent adjacent tokens are difficult to generate together, as their independent sampling may lead to inconsistencies. Based on this observation, we develop a parallel generation strategy that generates distant tokens with weak dependencies in parallel while maintaining sequential generation for strongly dependent local tokens. Our approach can be seamlessly integrated into standard autoregressive models without modifying the architecture or tokenizer. Experiments on ImageNet and UCF-101 demonstrate that our method achieves a 3.6x speedup with comparable quality and up to 9.5x speedup with minimal quality degradation across both image and video generation tasks. We hope this work will inspire future research in efficient visual generation and unified autoregressive modeling. Project page: https://epiphqny.github.io/PAR-project.

Autoregressive 이미지 생성의 병렬화 방법. 멀리 떨어진 토큰들은 상관 관계가 낮기 때문에 병렬로 생성 가능하다는 아이디어입니다. Locality를 활용한 병렬화를 얼마 전 연구에서도 시도했죠. (https://arxiv.org/abs/2412.04062) Permuted Autoregressive 모델에서 시도한 병렬 생성도 그렇고 (https://arxiv.org/abs/2412.01827) 추론 효율화는 어떻게든 결과가 나오는군요.

<english>
Parallelization of autoregressive image generation. As distant tokens has low correlations it is possible to generate in parallel. Actually parallelization using locality also tried on recent study (https://arxiv.org/abs/2412.04062). Considering parallelization tried in permuted autoregressive models ((https://arxiv.org/abs/2412.01827) It seems that it is always possible to make inference efficient.
</english>

#autoregressive-model #efficiency

# Links

[[241202 RandAR.md]]