https://arxiv.org/abs/2503.13751

*Optimizing ML Training with Metagradient Descent* (Logan Engstrom, Andrew Ilyas, Benjamin Chen, Axel Feldmann, William Moses, Aleksander Madry)

> A major challenge in training large-scale machine learning models is configuring the training process to maximize model performance, i.e., finding the best training setup from a vast design space. In this work, we unlock a gradient-based approach to this problem. We first introduce an algorithm for efficiently calculating metagradients -- gradients through model training -- at scale. We then introduce a "smooth model training" framework that enables effective optimization using metagradients. With metagradient descent (MGD), we greatly improve on existing dataset selection methods, outperform accuracy-degrading data poisoning attacks by an order of magnitude, and automatically find competitive learning rate schedules.

모델 학습 과정에 대한 그래디언트인 Metagradient로 데이터 선택 같은 하이퍼파라미터 최적화를 시도. 이 계통 아이디어는 정말 오랜만이네요.

<english>
Attempt to optimize hyperparameters like data selection using metagradient which is gradient of model training processes. It is long time I have seen these kind of ideas.
</english>

#hyperparameter 