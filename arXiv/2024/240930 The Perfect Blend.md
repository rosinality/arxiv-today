https://arxiv.org/abs/2409.20370

*The Perfect Blend: Redefining RLHF with Mixture of Judges* (Tengyu Xu, Eryk Helenowski, Karthik Abinav Sankararaman, Di Jin, Kaiyan Peng, Eric Han, Shaoliang Nie, Chen Zhu, Hejia Zhang, Wenxuan Zhou, Zhouhao Zeng, Yun He, Karishma Mandyam, Arya Talabzadeh, Madian Khabsa, Gabriel Cohen, Yuandong Tian, Hao Ma, Sinong Wang, Han Fang)

> Reinforcement learning from human feedback (RLHF) has become the leading approach for fine-tuning large language models (LLM). However, RLHF has limitations in multi-task learning (MTL) due to challenges of reward hacking and extreme multi-objective optimization (i.e., trade-off of multiple and/or sometimes conflicting objectives). Applying RLHF for MTL currently requires careful tuning of the weights for reward model and data combinations. This is often done via human intuition and does not generalize. In this work, we introduce a novel post-training paradigm which we called Constrained Generative Policy Optimization (CGPO). The core of CGPO is Mixture of Judges (MoJ) with cost-efficient constrained policy optimization with stratification, which can identify the perfect blend in RLHF in a principled manner. It shows strong empirical results with theoretical guarantees, does not require extensive hyper-parameter tuning, and is plug-and-play in common post-training pipelines. Together, this can detect and mitigate reward hacking behaviors while reaching a pareto-optimal point across an extremely large number of objectives. Our empirical evaluations demonstrate that CGPO significantly outperforms standard RLHF algorithms like PPO and DPO across various tasks including general chat, STEM questions, instruction following, and coding. Specifically, CGPO shows improvements of 7.4% in AlpacaEval-2 (general chat), 12.5% in Arena-Hard (STEM & reasoning), and consistent gains in other domains like math and coding. Notably, PPO, while commonly used, is prone to severe reward hacking in popular coding benchmarks, which CGPO successfully addresses. This breakthrough in RLHF not only tackles reward hacking and extreme multi-objective optimization challenges but also advances the state-of-the-art in aligning general-purpose LLMs for diverse applications.

현재 RLHF의 난점을 Multitask의 측면에서 생각했네요. Multitask에 대한 Reward Signal을 주어야 한다는 것과 이를 통해 RLHF를 진행해야 하는 것이 난이도를 높인다는 것입니다.

이에 대한 대응 방법으로 제약 조건을 부과하는 방법을 고안했네요. 예컨대 수학 문제라면 정답이 맞아야 한다는 것이 제약 조건이 되는 것이죠. 이에 더해 Reward Score를 캘리브레이션하는 방법을 설계했습니다.

그리고 프롬프트를 범주로 나눈 다음 각 카테고리에 대해 적합한 Judge를 적용하고 각 과제에 대한 그래디언트를 결합해 RLHF를 진행하는 형태입니다. 과제에 따라 KL Penalty 같은 하이퍼파라미터에도 차이를 줬군요.

Llama 3에서 다양한 과제에 대해 범주를 나눠 Preference를 수집하는 작업을 진행했었으니 그런 범주를 활용하는 방법을 생각하는 것도 자연스러운 것 같네요.

<english>
This paper approaches the current challenges of RLHF from the aspect of multitask learning. The difficulty lies in providing reward signals for multitask scenarios and then conducting RLHF based on these signals.

To address this issue, the authors devised a method that imposes constraints on the RLHF optimization process. For example, in mathematical problems, the constraint would be that the answer must be correct. Additionally, they designed a method to calibrate reward scores.

The approach then categorizes prompts and applies appropriate judges to each category. RLHF is then performed by combining the gradients from each task. Also, they varied hyperparameters like the KL penalty for different tasks.

Given that Llama 3 collected preferences for various tasks and categorized them, it seems natural to utilize such categorical structures.
</english>

#rlhf #multitask 