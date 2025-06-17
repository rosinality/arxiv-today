https://arxiv.org/abs/2410.23168

*TokenFormer: Rethinking Transformer Scaling with Tokenized Model Parameters* (Haiyang Wang, Yue Fan, Muhammad Ferjad Naeem, Yongqin Xian, Jan Eric Lenssen, Liwei Wang, Federico Tombari, Bernt Schiele)

> Transformers have become the predominant architecture in foundation models due to their excellent performance across various domains. However, the substantial cost of scaling these models remains a significant concern. This problem arises primarily from their dependence on a fixed number of parameters within linear projections. When architectural modifications (e.g., channel dimensions) are introduced, the entire model typically requires retraining from scratch. As model sizes continue growing, this strategy results in increasingly high computational costs and becomes unsustainable. To overcome this problem, we introduce TokenFormer, a natively scalable architecture that leverages the attention mechanism not only for computations among input tokens but also for interactions between tokens and model parameters, thereby enhancing architectural flexibility. By treating model parameters as tokens, we replace all the linear projections in Transformers with our token-parameter attention layer, where input tokens act as queries and model parameters as keys and values. This reformulation allows for progressive and efficient scaling without necessitating retraining from scratch. Our model scales from 124M to 1.4B parameters by incrementally adding new key-value parameter pairs, achieving performance comparable to Transformers trained from scratch while greatly reducing training costs. Code and models are available at \url{https://github.com/Haiyang-W/TokenFormer}.

트랜스포머의 Linear 레이어들을 학습 가능한 Key/Value 행렬과 토큰 사이의 Attention으로 대체. 과거 Learnable Key/Value로 Feed Forward를 대체할 수 있다는 연구가 생각나네요. (https://arxiv.org/abs/1907.01470) 이런 선택의 장점은 Key/Value 행렬의 토큰 크기를 늘리는 것으로 모델의 규모를 쉽게 확장시킬 수 있다는 것이죠. 재미있네요.

<english>
Replacing linear layers of transformer to learnable key/value matrices and attention between tokens. It reminds me previous study that we can replace feed forward with learnable key/value. (https://arxiv.org/abs/1907.01470) Benefit of this design is that by increasing number of tokens in key/value matrices we can easily scale-up the model. Intersting.
</english>

#transformer

# Links

