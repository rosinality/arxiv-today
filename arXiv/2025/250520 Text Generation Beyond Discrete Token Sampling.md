https://arxiv.org/abs/2505.14827

*Text Generation Beyond Discrete Token Sampling* (Yufan Zhuang, Liyuan Liu, Chandan Singh, Jingbo Shang, Jianfeng Gao)

> In standard autoregressive generation, an LLM predicts the next-token distribution, samples a discrete token, and then discards the distribution, passing only the sampled token as new input. To preserve this distribution's rich information, we propose Mixture of Inputs (MoI), a training-free method for autoregressive generation. After generating a token following the standard paradigm, we construct a new input that blends the generated discrete token with the previously discarded token distribution. Specifically, we employ a Bayesian estimation method that treats the token distribution as the prior, the sampled token as the observation, and replaces the conventional one-hot vector with the continuous posterior expectation as the new model input. MoI allows the model to maintain a richer internal representation throughout the generation process, resulting in improved text quality and reasoning capabilities. On mathematical reasoning, code generation, and PhD-level QA tasks, MoI consistently improves performance across multiple models including QwQ-32B, Nemotron-Super-49B, Gemma-3-27B, and DAPO-Qwen-32B, with no additional training and negligible computational overhead.

Continuous Thought. 추론 모델에 대해서 학습 없이 출력 토큰 분포로 임베딩을 가중합해서 입력으로 썼군요. Weight Merging과 연관이 있을지도 모르겠군요. 비슷한 접근이 같이 나왔습니다 (https://arxiv.org/abs/2505.15778).

<english>
Continous thought. The method is using weighted combination of embeddings using output token distribution for reasoning LMs, without training. Maybe it is related to weight merging. Similar approach also came out (https://arxiv.org/abs/2505.15778).
</english>

#reasoning 