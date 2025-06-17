https://arxiv.org/abs/2401.01325

LLM Maybe LongLM: Self-Extend LLM Context Window Without Tuning (Hongye Jin, Xiaotian Han, Jingfeng Yang, Zhimeng Jiang, Zirui Liu, Chia-Yuan Chang, Huiyuan Chen, Xia Hu)

Local한 영역에 대해 Positional Encoding을 그대로 사용하고, 그 밖의 영역은 Position을 나눠서 여러 토큰이 같은 Position을 공유하게 하는 동시에 최대 Position 값을 제한했군요. Perplexity 커브를 보면 (자주 그렇듯) 모델이 폭발하는 것을 막는 쪽에 가까운 느낌인데 폭발을 막는 것만으로도 확보할 수 있는 성능 향상이 있긴 하네요.

#long_context 