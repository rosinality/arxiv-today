https://arxiv.org/abs/2309.15098

Attention Satisfies: A Constraint-Satisfaction Lens on Factual Errors of Language Models (Mert Yuksekgonul, Varun Chandrasekaran, Erik Jones, Suriya Gunasekar, Ranjita Naik, Hamid Palangi, Ece Kamar, Besmira Nushi)

질문에 대해 사실로 답한 경우와 그렇지 않은 경우에 트랜스포머 내부에는 어떤 차이가 있을까? 여기서는 질문의 제약 조건, 예를 들어 Bad Romance를 부른 사람이 누구인가라는 질문에서의 Bad Romance와 같이 답변해야 하는 사람 혹은 대상(엔티티)을 한정하는 토큰에 대해 Attention 가중치가 어떠한가에 주목했네요. 사실을 답할 때 이 제약 조건에 대한 Attention 가중치가 그렇지 않을 때에 비해 높다고 합니다. 그리고 이 가중치를 사용해 사실을 답했는지 아닌지를 구분하는 것이 가능하다고 하는 군요.

대답해야 할 사람이 유명한 경우, 즉 코퍼스에서 흔히 등장할 법한 경우에 정답 확률이 높아진다는 것을 보면 어제 소개한 Embers of Autoregression (https://arxiv.org/abs/2309.13638) 이 떠오르는 군요.

#llm #transformer

# Links

[[230924 Embers of Autoregression.md]]