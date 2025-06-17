https://arxiv.org/abs/2401.10020

*Self-Rewarding Language Models* (Weizhe Yuan, Richard Yuanzhe Pang, Kyunghyun Cho, Sainbayar Sukhbaatar, Jing Xu, Jason Weston)

> We posit that to achieve superhuman agents, future models require superhuman feedback in order to provide an adequate training signal. Current approaches commonly train reward models from human preferences, which may then be bottlenecked by human performance level, and secondly these separate frozen reward models cannot then learn to improve during LLM training. In this work, we study Self-Rewarding Language Models, where the language model itself is used via LLM-as-a-Judge prompting to provide its own rewards during training. We show that during Iterative DPO training that not only does instruction following ability improve, but also the ability to provide high-quality rewards to itself. Fine-tuning Llama 2 70B on three iterations of our approach yields a model that outperforms many existing systems on the AlpacaEval 2.0 leaderboard, including Claude 2, Gemini Pro, and GPT-4 0613. While only a preliminary study, this work opens the door to the possibility of models that can continually improve in both axes.

일단 SFT 데이터와 평가 능력을 탑재하기 위한 데이터로 SFT를 합니다. 그 다음 모델로 프롬프트와 그에 대한 응답 샘플을 뽑은 다음 모델 자신이 응답을 평가하게 합니다. 평가한 결과를 사용해 DPO 스타일로 학습하죠. 튜닝된 모델을 사용해 이 과정을 반복합니다.

반복할수록 모델 성능이 향상된다는 것이 나타났군요. Policy 뿐만 아니라 Reward Model 또한 튜닝 과정에서 성능이 향상된다는 것이 포인트라고 할 수 있겠습니다. 단순하면서도 많은 생각을 해보게 하는 아이디어네요.

#alignment #feedback 