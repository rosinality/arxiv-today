https://arxiv.org/abs/2505.05713

*Understanding Stragglers in Large Model Training Using What-if Analysis* (Jinkun Lin, Ziheng Jiang, Zuquan Song, Sida Zhao, Menghan Yu, Zhanghan Wang, Chenyuan Wang, Zuocheng Shi, Xiang Shi, Wei Jia, Zherui Liu, Shuguang Wang, Haibin Lin, Xiu Liu, Aurojit Panda, Jinyang Li)

> Large language model (LLM) training is one of the most demanding distributed computations today, often requiring thousands of GPUs with frequent synchronization across machines. Such a workload pattern makes it susceptible to stragglers, where the training can be stalled by few slow workers. At ByteDance we find stragglers are not trivially always caused by hardware failures, but can arise from multiple complex factors. This work aims to present a comprehensive study on the straggler issues in LLM training, using a five-month trace collected from our ByteDance LLM training cluster. The core methodology is what-if analysis that simulates the scenario without any stragglers and contrasts with the actual case. We use this method to study the following questions: (1) how often do stragglers affect training jobs, and what effect do they have on job performance; (2) do stragglers exhibit temporal or spatial patterns; and (3) what are the potential root causes for stragglers?

대규모 모델 학습의 성능을 저하시키는 원인(Straggler)에 대한 분석. 각 워커에서 문제가 생기는 것보다는 시퀀스 길이의 불균등 같은 과제 자체의 문제와 가비지 컬렉터 등의 문제가 크다고 하는군요.

<english>
Analysis on stragglers, which reduced training performances in large scale model training. Rather than problems occur from individual workers, problem of task itself like imbalancedness of sequences lengths or garbage collector is more prominent problem.
</english>

#efficiency 