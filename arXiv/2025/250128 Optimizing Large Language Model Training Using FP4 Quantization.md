https://arxiv.org/abs/2501.17116

*Optimizing Large Language Model Training Using FP4 Quantization* (Ruizhe Wang, Yeyun Gong, Xiao Liu, Guoshuai Zhao, Ziyue Yang, Baining Guo, Zhengjun Zha, Peng Cheng)

> The growing computational demands of training large language models (LLMs) necessitate more efficient methods. Quantized training presents a promising solution by enabling low-bit arithmetic operations to reduce these costs. While FP8 precision has demonstrated feasibility, leveraging FP4 remains a challenge due to significant quantization errors and limited representational capacity. This work introduces the first FP4 training framework for LLMs, addressing these challenges with two key innovations: a differentiable quantization estimator for precise weight updates and an outlier clamping and compensation strategy to prevent activation collapse. To ensure stability, the framework integrates a mixed-precision training scheme and vector-wise quantization. Experimental results demonstrate that our FP4 framework achieves accuracy comparable to BF16 and FP8, with minimal degradation, scaling effectively to 13B-parameter LLMs trained on up to 100B tokens. With the emergence of next-generation hardware supporting FP4, our framework sets a foundation for efficient ultra-low precision training.

FP4 학습에 대한 연구. Straight Through Estimator에서 도함수를 Identity 대신 Quantization을 근사하는 함수로 바꾼 것이 주요하군요.

FP8 학습도 그렇게 널리 사용되는 것 같지는 않습니다만 블랙웰이 등장했으니 FP4 혹은 FP6 학습에 대한 연구도 계속 등장할 것 같네요.

The study on FP4 training. The key change is replacing the identity function in the straight through estimator's derivative with a function that approximates quantization.

I think even FP8 training hasn't become very widespread yet. But with the introduction of Blackwell, I expect we'll continue to see more research on FP4 and FP6 training.

#quantization #efficient-training 