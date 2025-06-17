https://arxiv.org/abs/2409.15156

*Rethinking Conventional Wisdom in Machine Learning: From Generalization to Scaling* (Lechao Xiao)

> The remarkable success of large language pretraining and the discovery of scaling laws signify a paradigm shift in machine learning. Notably, the primary objective has evolved from minimizing generalization error to reducing approximation error, and the most effective strategy has transitioned from regularization (in a broad sense) to scaling up models. This raises a critical question: Do the established principles that proved successful in the generalization-centric era remain valid in this new era of scaling? This paper examines several influential regularization-based principles that may no longer hold true in the scaling-centric, large language model (LLM) era. These principles include explicit L2 regularization and implicit regularization through small batch sizes and large learning rates. Additionally, we identify a new phenomenon termed ``scaling law crossover,'' where two scaling curves intersect at a certain scale, implying that methods effective at smaller scales may not generalize to larger ones. Together, these observations highlight two fundamental questions within this new paradigm: • Guiding Principles for Scaling: If regularization is no longer the primary guiding principle for model design, what new principles are emerging to guide scaling? • Model Comparison at Scale: How to reliably and effectively compare models at the scale where only a single experiment is feasible?

과거 데이터가 적고 모델이 커서 학습셋에 대한 성능에는 문제가 없고 학습셋과 테스트셋에 대한 성능 차이가 문제가 됐던 시절(Generalization Gap)에서 데이터가 늘어나 학습셋과 테스트셋의 성능 차이에는 문제가 없고 학습셋에 대한 성능이 문제가 되는 시점, Scaling의 시대가 되면서 이전에 통용됐던 직관들이 맞지 않을 수 있다는 주장. Regularization이 필요하지 않고 오히려 해로운 상황이 된 것이죠.

그래서 큰 LR이나 작은 배치 크기가 좋다는 발상이 맞지 않는다는 이야기를 합니다.

그 이후 LR이나 Weight Decay의 Scaling 방법에 따라서 작은 규모에서는 문제가 없었던 방법들이 큰 규모로 가면서 문제가 발생하는 상황들에 대해 언급합니다. 그리고 이 때문에 큰 규모에서 모델과 하이퍼파라미터를 비교하는 것이 어렵다는 이야기를 하네요.

생각을 많이 해보게 되네요.

#scaling-law #hyperparameter