https://arxiv.org/abs/2505.16260

*Small-to-Large Generalization: Data Influences Models Consistently Across Scale* (Alaa Khaddaj, Logan Engstrom, Aleksander Madry)

> Choice of training data distribution greatly influences model behavior. Yet, in large-scale settings, precisely characterizing how changes in training data affects predictions is often difficult due to model training costs. Current practice is to instead extrapolate from scaled down, inexpensive-to-train proxy models. However, changes in data do not influence smaller and larger models identically. Therefore, understanding how choice of data affects large-scale models raises the question: how does training data distribution influence model behavior across compute scale? We find that small- and large-scale language model predictions (generally) do highly correlate across choice of training data. Equipped with these findings, we characterize how proxy scale affects effectiveness in two downstream proxy model applications: data attribution and dataset selection.

학습 데이터셋의 효과를 대상 모델보다 훨씬 작은 모델에서 추정할 수 있는가? Loss의 상관관계가 모델이 아주 작지 않다면 상당히 높다고 하네요. 심지어 과제 자체에 대한 성능이 무작위 수준인 경우에도 그렇다고 합니다.

<english>
Would it possible to estimate effect of training dataset using much smaller model compared to target models? The paper insist that correlation on losses are quite high unless model is too small. Even when performance on the task itself is on random level.
</english>

#dataset #scaling-law 