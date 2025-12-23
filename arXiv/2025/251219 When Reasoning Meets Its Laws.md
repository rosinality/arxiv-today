https://arxiv.org/abs/2512.17901

*When Reasoning Meets Its Laws* (Junyu Zhang, Yifan Sun, Tianang Leng, Jingyan Shen, Liu Ziyin, Paul Pu Liang, Huan Zhang)

> Despite the superior performance of Large Reasoning Models (LRMs), their reasoning behaviors are often counterintuitive, leading to suboptimal reasoning capabilities. To theoretically formalize the desired reasoning behaviors, this paper presents the Laws of Reasoning (LoRe), a unified framework that characterizes intrinsic reasoning patterns in LRMs. We first propose compute law with the hypothesis that the reasoning compute should scale linearly with question complexity. Beyond compute, we extend LoRe with a supplementary accuracy law. Since the question complexity is difficult to quantify in practice, we examine these hypotheses by two properties of the laws, monotonicity and compositionality. We therefore introduce LoRe-Bench, a benchmark that systematically measures these two tractable properties for large reasoning models. Evaluation shows that most reasoning models exhibit reasonable monotonicity but lack compositionality. In response, we develop an effective finetuning approach that enforces compute-law compositionality. Extensive empirical studies demonstrate that better compliance with compute laws yields consistently improved reasoning performance on multiple benchmarks, and uncovers synergistic effects across properties and laws. Project page: https://lore-project.github.io/

추론에 대해 기대되는 규칙성들.

1. 과제의 복잡성에 따라 추론의 길이는 단조 증가해야 한다.

2. 두 개의 과제가 독립적이라면 두 개 과제의 조합에 필요한 추론의 길이는 각 과제에 필요한 추론 길이의 합과 유사해야 한다.

추론 모델들은 단조적 특성은 나타내지만 조합에 따른 특성은 잘 나타나지 않음. 따라서 Compositionality를 강제하는 방향이 가능할지도.

Expected regularities of reasoning.

1. Reasoning length should increase monotonically with task complexity.

2. If two tasks are independent, composition of tasks requires reasoning length approximately similar to sum of reasoning lengths for each task.

Reasoning models tend to have monotonicity but lack compositionality. Therefore, maybe we can enforce compositionality.

#rl #reasoning 