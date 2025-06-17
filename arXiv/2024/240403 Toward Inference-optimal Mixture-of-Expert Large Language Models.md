https://arxiv.org/abs/2404.02852

*Toward Inference-optimal Mixture-of-Expert Large Language Models* (Longfei Yun, Yonghao Zhuang, Yao Fu, Eric P Xing, Hao Zhang)

> Mixture-of-Expert (MoE) based large language models (LLMs), such as the recent Mixtral and DeepSeek-MoE, have shown great promise in scaling model size without suffering from the quadratic growth of training cost of dense transformers. Like dense models, training MoEs requires answering the same question: given a training budget, what is the optimal allocation on the model size and number of tokens? We study the scaling law of MoE-based LLMs regarding the relations between the model performance, model size, dataset size, and the expert degree. Echoing previous research studying MoE in different contexts, we observe the diminishing return of increasing the number of experts, but this seems to suggest we should scale the number of experts until saturation, as the training cost would remain constant, which is problematic during inference time. We propose to amend the scaling law of MoE by introducing inference efficiency as another metric besides the validation loss. We find that MoEs with a few (4/8) experts are the most serving efficient solution under the same performance, but costs 2.5-3.5x more in training. On the other hand, training a (16/32) expert MoE much smaller (70-85%) than the loss-optimal solution, but with a larger training dataset is a promising setup under a training budget.

MoE Scaling Law와 비용 모델을 사용해 같은 Loss를 최소 비용으로 달성하는 Expert의 수가 얼마일지를 추정한 연구. Overtraining까지 고려하면 16 Expert 정도가 좋은 것 같다는 결론입니다.

다만 MoE Scaling Law, 비용 모델이 모두 맞아야 하고 MoE도 Expert의 크기를 줄이고 Top-K를 높이는 방식 등이 나오고 있어서 정확한 추정이 어려울 것 같긴 하네요. 다만 공교롭게도 요즘 나 MoE 모델들은 (Expert를 줄인 경우를 제외하면) 8, 16 Expert가 많긴 하군요.

#moe #scaling-law 