https://arxiv.org/abs/2501.03124

*PRMBench: A Fine-grained and Challenging Benchmark for Process-Level Reward Models* (Mingyang Song, Zhaochen Su, Xiaoye Qu, Jiawei Zhou, Yu Cheng)

> Process-level Reward Models (PRMs) are crucial for complex reasoning and decision-making tasks, where each intermediate step plays an important role in the reasoning process. Since language models are prone to various types of errors during the reasoning process, PRMs are required to possess nuanced capabilities for detecting various implicit error types in real-world scenarios. However, current benchmarks primarily focus on step correctness, failing to evaluate PRMs' performance systematically. To address this gap, we introduce PRMBench, a process-level benchmark specifically designed to assess the fine-grained error detection capabilities of PRMs. PRMBench comprises 6,216 carefully designed problems and 83,456 step-level labels, evaluating models across multiple dimensions, including simplicity, soundness, and sensitivity. In our experiments on 15 models, spanning both open-source PRMs and closed-source large language models prompted as critic models, we uncover significant weaknesses in current PRMs. These findings underscore the challenges inherent in process-level evaluation and highlight key directions for future research. We hope PRMBench can be a robust bench for advancing research on PRM evaluation and development.

PRM800K 기반으로 구축한 Process Reward Model에 대한 벤치마크. 각 스텝에 대한 평가에서 평가 기준 카테고리를 추가적으로 지정했다는 것이 재미있네요.

<english>
Benchmark for process reward models based on PRM800K. It is interesting that they added category of criteria for evaluating each steps.
</english>

#benchmark #reward-model 