https://arxiv.org/abs/2404.07647

*Why do small language models underperform? Studying Language Model Saturation via the Softmax Bottleneck* (Nathan Godey, Éric de la Clergerie, Benoît Sagot)

> Recent advances in language modeling consist in pretraining highly parameterized neural networks on extremely large web-mined text corpora. Training and inference with such models can be costly in practice, which incentivizes the use of smaller counterparts. However, it has been observed that smaller models can suffer from saturation, characterized as a drop in performance at some advanced point in training followed by a plateau. In this paper, we find that such saturation can be explained by a mismatch between the hidden dimension of smaller models and the high rank of the target contextual probability distribution. This mismatch affects the performance of the linear prediction head used in such models through the well-known softmax bottleneck phenomenon. We measure the effect of the softmax bottleneck in various settings and find that models based on less than 1000 hidden dimensions tend to adopt degenerate latent representations in late pretraining, which leads to reduced evaluation performance.

작은 LM에서 학습 후반에 성능이 감소하는 현상에 대한 분석. 이 문제의 원인을 Representation의 Anistropy로 짚고 있고 이를 Softmax Bottleneck과 연결하고 있네요. Contrastive Learning에서의 Rank Collapse 문제를 다시 떠오르게 하는 주제입니다.

#llm #contrastive-learning #representation 