https://arxiv.org/abs/2411.12925

*Loss-to-Loss Prediction: Scaling Laws for All Datasets* (David Brandfonbrener, Nikhil Anand, Nikhil Vyas, Eran Malach, Sham Kakade)

> While scaling laws provide a reliable methodology for predicting train loss across compute scales for a single data distribution, less is known about how these predictions should change as we change the distribution. In this paper, we derive a strategy for predicting one loss from another and apply it to predict across different pre-training datasets and from pre-training data to downstream task data. Our predictions extrapolate well even at 20x the largest FLOP budget used to fit the curves. More precisely, we find that there are simple shifted power law relationships between (1) the train losses of two models trained on two separate datasets when the models are paired by training compute (train-to-train), (2) the train loss and the test loss on any downstream distribution for a single model (train-to-test), and (3) the test losses of two models trained on two separate train datasets (test-to-test). The results hold up for pre-training datasets that differ substantially (some are entirely code and others have no code at all) and across a variety of downstream tasks. Finally, we find that in some settings these shifted power law relationships can yield more accurate predictions than extrapolating single-dataset scaling laws.

아주 흥미로운 결과네요. 하나의 데이터셋에 대한 Loss를 다른 데이터셋에 대한 Loss로 변환하는 Scaling Law입니다. 따라서 학습 데이터셋 사이에서 또는 학습 데이터셋과 평가 데이터셋에서, 그리고 서로 다른 데이터셋에 대해 학습한 모델의 평가 데이터셋에 대한 Loss의 관계를 추정할 수 있습니다.

기본적인 함수형은 Kaplan Scaling Law를 엔트로피의 하한으로 평행이동하고 지수를 도입한 형태네요.

<english>
Very intriguing results. Scaling law that transforms loss from one dataset to another. So we can estimate relationship between training datasets, or training and test sets, or even models trained with different datasets and evaluated on another test sets.

Basic functional form is shifting Kaplan scaling law with irreducible entropy and introduce exponent.
</english>

#scaling-law 