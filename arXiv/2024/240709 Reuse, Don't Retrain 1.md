https://arxiv.org/abs/2407.07263

*Reuse, Don't Retrain: A Recipe for Continued Pretraining of Language Models* (Jupinder Parmar, Sanjev Satheesh, Mostofa Patwary, Mohammad Shoeybi, Bryan Catanzaro)

> As language models have scaled both their number of parameters and pretraining dataset sizes, the computational cost for pretraining has become intractable except for the most well-resourced teams. This increasing cost makes it ever more important to be able to reuse a model after it has completed pretraining; allowing for a model's abilities to further improve without needing to train from scratch. In this work, we detail a set of guidelines that cover how to design efficacious data distributions and learning rate schedules for continued pretraining of language models. When applying these findings within a continued pretraining run on top of a well-trained 15B parameter model, we show an improvement of 9\% in average model accuracy compared to the baseline of continued training on the pretraining set. The resulting recipe provides a practical starting point with which to begin developing language models through reuse rather than retraining.

NVIDIA의 Continual Pretraining 실험인데 다른 언어에 학습시킨다거나 하는 세팅이 아니라 QA 데이터셋에 학습시키는 과제네요. 학습 초반에는 분포가 같은 프리트레이닝 데이터를 쓰다가 후반에 QA 데이터를 사용한다, 구간을 나눠 후반에는 높은 퀄리티의 데이터만 사용한다 등등의 방법들인데 약간 Continual Pretraining보다도 학습 단계를 나누는 접근처럼 느껴지기도 하네요.

#continual-learning #pretraining 