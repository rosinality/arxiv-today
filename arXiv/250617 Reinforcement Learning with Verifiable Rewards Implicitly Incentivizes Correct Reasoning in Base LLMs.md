https://arxiv.org/abs/2506.14245

*Reinforcement Learning with Verifiable Rewards Implicitly Incentivizes Correct Reasoning in Base LLMs* (Xumeng Wen, Zihan Liu, Shun Zheng, Zhijian Xu, Shengyu Ye, Zhirong Wu, Xiao Liang, Yang Wang, Junjie Li, Ziming Miao, Jiang Bian, Mao Yang)

> Reinforcement Learning with Verifiable Rewards (RLVR) has emerged as a promising paradigm for advancing the reasoning capabilities of Large Language Models (LLMs). However, a critical paradox clouds its efficacy: RLVR-tuned models often underperform their base models on the $Pass@K$ metric for solution-finding, leading to the hypothesis that RLVR merely re-weights existing reasoning paths at the cost of reasoning diversity. In this work, we resolve this contradiction by identifying the source of the problem: the $Pass@K$ metric itself is a flawed measure of reasoning, as it credits correct final answers that probably arise from inaccurate or incomplete chains of thought (CoTs). To address this, we introduce a more precise evaluation metric, $CoT$-$Pass@K$, which mandates that both the reasoning path and the final answer be correct. We provide a new theoretical foundation that formalizes how RLVR, unlike traditional RL, is uniquely structured to incentivize logical integrity. Our empirical results are supportive: using $CoT$-$Pass@K$, we observe that RLVR can incentivize the generalization of correct reasoning for all values of $K$. Furthermore, by analyzing the training dynamics, we find that this enhanced reasoning capability emerges early in the training process and smoothly generalizes. Our work provides a clear perspective on the role of RLVR, offers a more reliable method for its evaluation, and confirms its potential to genuinely advance machine reasoning.

Pass@K를 기반으로 추론 RL이 정답에 필요한 샘플의 수와 다양성을 감소시키는 형태로 동작한다는 주장이 있었죠 (https://arxiv.org/abs/2504.13837). 여기서는 CoT의 내용이 올바른지도 체크하면 패턴이 달라진다는 주장을 합니다. 사실 Pass@K 자체가 베이스라인에 대한 고려가 필요한 지표죠 (https://arxiv.org/abs/2410.15466).

<english>
There was suggestion that reasoning RL works by reducing samples required for correct answer, and diversity, based on pass@K (https://arxiv.org/abs/2504.13837). This study insists that pattern is changed if we check content of CoT itself is correct. Actually pass@K itself is a metric requires considering baseline (https://arxiv.org/abs/2410.15466).
</english>

#rl #reasoning 