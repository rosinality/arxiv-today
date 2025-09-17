https://arxiv.org/abs/2508.19228

*Predicting the Order of Upcoming Tokens Improves Language Modeling* (Zayd M. K. Zuhri, Erland Hilman Fuadi, Alham Fikri Aji)

> Multi-Token Prediction (MTP) has been proposed as an auxiliary objective to improve next-token prediction (NTP) in language model training but shows inconsistent improvements, underperforming in standard NLP benchmarks. We argue that MTP's exact future token prediction is too difficult as an auxiliary loss. Instead, we propose Token Order Prediction (TOP), which trains models to order upcoming tokens by their proximity using a learning-to-rank loss. TOP requires only a single additional unembedding layer compared to MTP's multiple transformer layers. We pretrain models of 340M, 1.8B, and 7B parameters using NTP, MTP, and TOP objectives. Results on eight standard NLP benchmarks show that TOP overall outperforms both NTP and MTP even at scale. Our code is available at https://github.com/zaydzuhri/token-order-prediction

Multiple Token Prediction이 너무 어려운 과제일 수 있다는 아이디어. 대신 모델이 Window 내의 토큰들 사이의 거리를 예측하게 함.

Multiple token prediction could be too hard, so instead let the model predict the distance between tokens in the window.

#autoregressive-model 