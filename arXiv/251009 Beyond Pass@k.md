https://arxiv.org/abs/2510.08325

*Beyond Pass@k: Breadth-Depth Metrics for Reasoning Boundaries* (Marius Dragoi, Ioana Pintilie, Florin Gogianu, Florin Brad)

> Reinforcement Learning with Verifiable Rewards (RLVR) has emerged as a powerful paradigm to improve Large Language Models on reasoning tasks such as coding, math or logic. To assess the reasoning boundary (the fraction of problems a model can solve) researchers often report Pass@k at large sampling budgets. Recent results reveal a crossover phenomenon: while RLVR models outperform the base model at small k values, the base model usually outperforms them when sampling a very large number of completions. This has been interpreted as evidence that base models have a larger reasoning boundary. We argue that on tasks with discrete answer spaces, such as math with numeric outputs, Pass@k at large k reflects the increasingly higher chance of success in the limit of the number of trials rather than genuine reasoning, and can therefore be misleading. We propose Cover@tau, which measures the fraction of problems that a model can solve for which at least a tau proportion of completions are correct. Unlike Pass@k, Cover@tau captures reasoning under an explicit reliability threshold: models that rely on random guessing degrade rapidly as tau increases. We evaluate several RLVR models using Cover@tau-based metrics and illustrate how the relative rankings of popular algorithms change compared to Pass@1, offering a different perspective on reasoning boundaries.

Pass@K의 베이스라인 문제를 해소하기 위한 새로운 척도. 특정 역치 이상의 확률로 풀 수 있는 문제의 비율을 측정.

<english>
Designing new metric to resolve baseline problem of Pass@K. This metric measures the fraction of problems that can be solved with probability more than certain threshold.
</english>

#benchmark 