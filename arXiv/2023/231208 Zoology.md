https://arxiv.org/abs/2312.04927

Zoology: Measuring and Improving Recall in Efficient Language Models (Simran Arora, Sabri Eyuboglu, Aman Timalsina, Isys Johnson, Michael Poli, James Zou, Atri Rudra, Christopher Ré)

https://hazyresearch.stanford.edu/blog/2023-12-11-zoology1-analysis

Attention과 State Space Model의 중요한 차이는 Attention에서는 각 토큰에서 필요한 정보를 이전 토큰들에서 찾아올 수 있다는 것이죠. 그 차이가 가장 잘 드러나는 것이 Associative Recall, 즉 컨텍스트에서 나타나는 패턴을 가져올 수 있는 능력이죠. Attention은 이걸 아주 쉽게 풀 수 있지만 State Space Model에서는 State의 차원이 길이에 따라 증가해야만 가능하죠.

대안은 무엇인가? 하면 역시 Attention을 몇 개 붙여주는 것이 가장 좋은 것처럼 보이네요. Multi-head Long Convolution (Hyena) (https://arxiv.org/abs/2310.18780) 도 이 문제에 대해서는 도움이 되는 것으로 보입니다. Striped Hyena 같은 Long Convolution과 Attention의 절충이 트랜스포머보다 실제로 나을 수 있다는 생각이 드네요.

#state_space_model #attention

# Links

