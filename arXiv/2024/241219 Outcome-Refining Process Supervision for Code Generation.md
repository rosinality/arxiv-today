https://arxiv.org/abs/2412.15118

*Outcome-Refining Process Supervision for Code Generation* (Zhuohao Yu, Weizheng Gu, Yidong Wang, Zhengran Zeng, Jindong Wang, Wei Ye, Shikun Zhang)

> Large Language Models have demonstrated remarkable capabilities in code generation, yet they often struggle with complex programming tasks that require deep algorithmic reasoning. While process supervision through learned reward models shows promise in guiding reasoning steps, it requires expensive training data and suffers from unreliable evaluation. We propose Outcome-Refining Process Supervision, a novel paradigm that treats outcome refinement itself as the process to be supervised. Our framework leverages concrete execution signals to ground the supervision of reasoning steps, while using tree-structured exploration to maintain multiple solution trajectories simultaneously. Experiments demonstrate that our approach enables even smaller models to achieve high success accuracy and performance metrics on competitive programming tasks, creates more reliable verification than traditional reward models without requiring training PRMs. Our approach achieves significant improvements across 5 models and 3 datasets: an average of 26.9% increase in correctness and 42.2% in efficiency. The results suggest that providing structured reasoning space with concrete verification signals is crucial for solving complex programming tasks. We open-source all our code and data at: https://github.com/zhuohaoyu/ORPS

Execution 피드백과 Process Reward의 결합. 샘플링 후 생성된 코드를 실행하고 실행 결과에 대한 Critique을 생성해 피드백을 주는 구조군요.

Process Reward를 사용한다고 하더라도 각 스텝에 대한 점수를 주는 것을 넘어 그 스텝에 대한 추론 과정이 필요하다는 생각을 합니다. 그러면 PRM이 Critic 모델에 가까워지겠죠.

<english>
Combination of execution feedback and process reward. Execute the code after sampling and give a feedback by generating critique with respect to execution results.

I think even when we use process reward, we need reasonings for each steps beyond just scoring it. Then PRM would became similar to critic models.
</english>

#reward-model #search #code 