https://arxiv.org/abs/2504.11393

*DataDecide: How to Predict Best Pretraining Data with Small Experiments* (Ian Magnusson, Nguyen Tai, Ben Bogin, David Heineman, Jena D. Hwang, Luca Soldaini, Akshita Bhagia, Jiacheng Liu, Dirk Groeneveld, Oyvind Tafjord, Noah A. Smith, Pang Wei Koh, Jesse Dodge)

> Because large language models are expensive to pretrain on different datasets, using smaller-scale experiments to decide on data is crucial for reducing costs. Which benchmarks and methods of making decisions from observed performance at small scale most accurately predict the datasets that yield the best large models? To empower open exploration of this question, we release models, data, and evaluations in DataDecide -- the most extensive open suite of models over differences in data and scale. We conduct controlled pretraining experiments across 25 corpora with differing sources, deduplication, and filtering up to 100B tokens, model sizes up to 1B parameters, and 3 random seeds. We find that the ranking of models at a single, small size (e.g., 150M parameters) is a strong baseline for predicting best models at our larger target scale (1B) (~80% of com parisons correct). No scaling law methods among 8 baselines exceed the compute-decision frontier of single-scale predictions, but DataDecide can measure improvement in future scaling laws. We also identify that using continuous likelihood metrics as proxies in small experiments makes benchmarks including MMLU, ARC, HellaSwag, MBPP, and HumanEval >80% predictable at the target 1B scale with just 0.01% of the compute.

프리트레이닝을 위한 최적의 데이터 구성을 소규모 연산으로 찾는 방법. Scaling Law 추정 대신 하나의 규모에서 실험하고 최적 레시피를 찾는 것이 효과적이었다고 하네요.

<english>
Finding optimal data composition for pretraining using small scale computation. The study suggests that instead of estimating scaling law experimenting in a single scale and find out optimal recipe was effective.
</english>

#scaling-law #pretraining 