https://arxiv.org/abs/2502.15950

*Optimizing Pre-Training Data Mixtures with Mixtures of Data Expert Models* (Lior Belenki, Alekh Agarwal, Tianze Shi, Kristina Toutanova)

> We propose a method to optimize language model pre-training data mixtures through efficient approximation of the cross-entropy loss corresponding to each candidate mixture via a Mixture of Data Experts (MDE). We use this approximation as a source of additional features in a regression model, trained from observations of model loss for a small number of mixtures. Experiments with Transformer decoder-only language models in the range of 70M to 1B parameters on the SlimPajama dataset show that our method achieves significantly better performance than approaches that train regression models using only the mixture rates as input features. Combining this improved optimization method with an objective that takes into account cross-entropy on end task data leads to superior performance on few-shot downstream evaluations. We also provide theoretical insights on why aggregation of data expert predictions can provide good approximations to model losses for data mixtures.

프리트레이닝 데이터의 비율 결정. 각 도메인에 대해 모델을 학습시킨 다음 이 모델을 특정 비율로 앙상블했을 때 가장 좋은 비율을 사용한다는 아이디어.

<english>
Determining ratio of pretraining domains. After training a model on each domains and use best ratios from ensemble of each models with specific mixture ratios.
</english>

#pretraining 