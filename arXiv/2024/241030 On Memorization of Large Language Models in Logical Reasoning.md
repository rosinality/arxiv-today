https://arxiv.org/abs/2410.23123

*On Memorization of Large Language Models in Logical Reasoning* (Chulin Xie, Yangsibo Huang, Chiyuan Zhang, Da Yu, Xinyun Chen, Bill Yuchen Lin, Bo Li, Badih Ghazi, Ravi Kumar)

> Large language models (LLMs) achieve good performance on challenging reasoning benchmarks, yet could also make basic reasoning mistakes. This contrasting behavior is puzzling when it comes to understanding the mechanisms behind LLMs' reasoning capabilities. One hypothesis is that the increasingly high and nearly saturated performance on common reasoning benchmarks could be due to the memorization of similar problems. In this paper, we systematically investigate this hypothesis with a quantitative measurement of memorization in reasoning tasks, using a dynamically generated logical reasoning benchmark based on Knights and Knaves (K&K) puzzles. We found that LLMs could interpolate the training puzzles (achieving near-perfect accuracy) after fine-tuning, yet fail when those puzzles are slightly perturbed, suggesting that the models heavily rely on memorization to solve those training puzzles. On the other hand, we show that while fine-tuning leads to heavy memorization, it also consistently improves generalization performance. In-depth analyses with perturbation tests, cross difficulty-level transferability, probing model internals, and fine-tuning with wrong answers suggest that the LLMs learn to reason on K&K puzzles despite training data memorization. This phenomenon indicates that LLMs exhibit a complex interplay between memorization and genuine reasoning abilities. Finally, our analysis with per-sample memorization score sheds light on how LLMs switch between reasoning and memorization in solving logical puzzles. Our code and data are available at https://memkklogic.github.io.

암기 vs 추론. 추론 과제로 파인튜닝을 했을 때 Perturbation을 통해 모델이 문제를 암기 혹은 추론 중 둘 중 어느 쪽으로 해결하는지를 체크하면 암기를 통해 문제를 푸는 경향이 나타나지만 동시에 추론 능력을 통한 일반화 또한 나타난다는 연구. 난이도가 높아질수록 암기 경향이 강해지는 것도 직관적이군요.

<english>
Memorization vs reasoning. If we check how model solves the problem by applying perturbation after finetuning with reasoning tasks, then model have tendency to do memorization, but also generalization from reasonings. It is intuitive pattern that model tend to depend on memorization more if difficulty of proble is increased.
</english>

#reasoning 