https://arxiv.org/abs/2403.16952

*Data Mixing Laws: Optimizing Data Mixtures by Predicting Language Modeling Performance* (Jiasheng Ye, Peiju Liu, Tianxiang Sun, Yunhua Zhou, Jun Zhan, Xipeng Qiu)

> Pretraining data of large language models composes multiple domains (e.g., web texts, academic papers, codes), whose mixture proportions crucially impact the competence of outcome models. While existing endeavors rely on heuristics or qualitative strategies to tune the proportions, we discover the quantitative predictability of model performance regarding the mixture proportions in function forms, which we refer to as the data mixing laws. Fitting such functions on sample mixtures unveils model performance on unseen mixtures before actual runs, thus guiding the selection of an ideal data mixture. Furthermore, we propose nested use of the scaling laws of training steps, model sizes, and our data mixing law to enable predicting the performance of large models trained on massive data under various mixtures with only small-scale training. Moreover, experimental results verify that our method effectively optimizes the training mixture of a 1B model trained for 100B tokens in RedPajama, reaching a performance comparable to the one trained for 48% more steps on the default mixture. Extending the application of data mixing laws to continual training accurately predicts the critical mixture proportion that avoids catastrophic forgetting and outlooks the potential for dynamic data schedules

프리트레이닝 데이터셋 비율에 따른 Loss에 대한 Law. 사실 크기를 키우는 것과 관련된 Law는 아니라서 저자의 언급처럼 Scaling Law라고 말하기는 어렵겠네요.

기본적으로 도메인 i에 대한 Loss(i) = exp(ratio(i))라는 함수형입니다. 여기에 더해 이 도메인들을 종합한 데이터에 대한 Validation Loss를 구하는데 여기서 각 도메인의 비율을 알고 있지 않을 때에 대해서 적용할 수 있도록 Validation 셋이 가상의 도메인 K개로 구성되어 있다고 보고 추정합니다. 추정할 파라미터 수가 크게 늘어나는 감이 있긴 합니다.

Downstream 과제에 대한 Scaling Law (https://arxiv.org/abs/2403.08540) 와 결합하면 프리트레이닝 의사 결정에 좀 더 도움이 될 수도 있지 않을까 하는 생각이 있습니다.

#scaling-law

# Links

[[240313 Language models scale reliably with over-training and on downstream tasks.md]]