https://arxiv.org/abs/2406.07515

*Beyond Model Collapse: Scaling Up with Synthesized Data Requires Reinforcement* (Yunzhen Feng, Elvis Dohmatob, Pu Yang, Francois Charton, Julia Kempe)

> Synthesized data from generative models is increasingly considered as an alternative to human-annotated data for fine-tuning Large Language Models. This raises concerns about model collapse: a drop in performance of models fine-tuned on generated data. Considering that it is easier for both humans and machines to tell between good and bad examples than to generate high-quality samples, we investigate the use of feedback on synthesized data to prevent model collapse. We derive theoretical conditions under which a Gaussian mixture classification model can achieve asymptotically optimal performance when trained on feedback-augmented synthesized data, and provide supporting simulations for finite regimes. We illustrate our theoretical predictions on two practical problems: computing matrix eigenvalues with transformers and news summarization with large language models, which both undergo model collapse when trained on model-generated data. We show that training from feedback-augmented synthesized data, either by pruning incorrect predictions or by selecting the best of several guesses, can prevent model collapse, validating popular approaches like RLHF.

합성 데이터로 모델을 학습시키면 모델이 Collapse 하는데, 피드백 (샘플 선택) 메커니즘이 들어가면 성능 개선이 가능한가? 에 대한 연구. 가능하다고 합니다.

합성 데이터는 크게 두 가지 방향을 생각해볼 수 있겠죠.

1. 기존 데이터에서 더 많은 정보를 끌어내는 방법으로서의 합성 데이터.
2. 합성 데이터에 피드백 등으로 추가적인 정보를 주입하는 방법.

둘 모두 유망한 방법 듯 하고 두 영역 모두에서 중요한 진전들이 나오지 않을까 싶네요.

#synthetic-data 