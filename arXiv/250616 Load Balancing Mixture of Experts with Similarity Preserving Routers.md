https://arxiv.org/abs/2506.14038

*Load Balancing Mixture of Experts with Similarity Preserving Routers* (Nabil Omi, Siddhartha Sen, Ali Farhadi)

> Sparse Mixture of Experts (MoE) models offer a scalable and efficient architecture for training large neural networks by activating only a subset of parameters ("experts") for each input. A learned router computes a distribution over these experts, and assigns input tokens to a small subset. However, without auxiliary balancing mechanisms, routers often converge to using only a few experts, severely limiting model capacity and degrading performance. Most current load balancing mechanisms encourage a distribution over experts that resembles a roughly uniform distribution of experts per token. During training, this can result in inconsistent routing behavior, resulting in the model spending its capacity to learn redundant knowledge. We address this by introducing a novel load balancing loss that preserves token-wise relational structure, encouraging consistent expert choices for similar inputs during training. Our experimental results show that applying our loss to the router results in 36% faster convergence and lower redundancy compared to a popular load balancing loss.

MoE 라우터 가중치를 직교 행렬로 정규화하는 형태의 Load Balancing. 실제 Load Balancing이 얼마나 잘 되는지가 궁금하네요.

#moe 