https://arxiv.org/abs/2512.21625

*Rethinking Sample Polarity in Reinforcement Learning with Verifiable Rewards* (Xinyu Tang, Yuliang Zhan, Zhixun Li, Wayne Xin Zhao, Zhenduo Zhang, Zujie Wen, Zhiqiang Zhang, Jun Zhou)

> Large reasoning models (LRMs) are typically trained using reinforcement learning with verifiable reward (RLVR) to enhance their reasoning abilities. In this paradigm, policies are updated using both positive and negative self-generated rollouts, which correspond to distinct sample polarities. In this paper, we provide a systematic investigation into how these sample polarities affect RLVR training dynamics and behaviors. We find that positive samples sharpen existing correct reasoning patterns, while negative samples encourage exploration of new reasoning paths. We further explore how adjusting the advantage values of positive and negative samples at both the sample level and the token level affects RLVR training. Based on these insights, we propose an Adaptive and Asymmetric token-level Advantage shaping method for Policy Optimization, namely A3PO, that more precisely allocates advantage signals to key tokens across different polarities. Experiments across five reasoning benchmarks demonstrate the effectiveness of our approach.

Positive와 Negative 샘플이 엔트로피와 응답 길이에 미치는 영향에 대한 추가 분석. 또한 엔트로피 혹은 확률 기반으로 Advantage Shaping을 사용해 토큰 레벨에서 분석.

More analysis on how positive or negative samples affect entropy and response length. They also analyzed this at the token level through advantage shaping, with entropy or probability.

#rl #reasoning 