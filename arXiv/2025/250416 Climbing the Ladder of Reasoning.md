https://arxiv.org/abs/2504.11741

*Climbing the Ladder of Reasoning: What LLMs Can-and Still Can't-Solve after SFT?* (Yiyou Sun, Georgia Zhou, Hao Wang, Dacheng Li, Nouha Dziri, Dawn Song)

> Recent supervised fine-tuning (SFT) approaches have significantly improved language models' performance on mathematical reasoning tasks, even when models are trained at a small scale. However, the specific capabilities enhanced through such fine-tuning remain poorly understood. In this paper, we conduct a detailed analysis of model performance on the AIME24 dataset to understand how reasoning capabilities evolve. We discover a ladder-like structure in problem difficulty, categorize questions into four tiers (Easy, Medium, Hard, and Extremely Hard (Exh)), and identify the specific requirements for advancing between tiers. We find that progression from Easy to Medium tier requires adopting an R1 reasoning style with minimal SFT (500-1K instances), while Hard-level questions suffer from frequent model's errors at each step of the reasoning chain, with accuracy plateauing at around 65% despite logarithmic scaling. Exh-level questions present a fundamentally different challenge; they require unconventional problem-solving skills that current models uniformly struggle with. Additional findings reveal that carefully curated small-scale datasets offer limited advantage-scaling dataset size proves far more effective. Our analysis provides a clearer roadmap for advancing language model capabilities in mathematical reasoning.

SFT를 사용해서 추론을 학습시켰을 때의 결과 분석. 쉬운 문제들은 적은 수의 SFT 샘플만으로도 빠르게 성능이 향상되는데, 어려운 문제들의 경우에는 훨씬 더 많은 샘플이 필요하다고 하는군요. RL에 대해서라면 어떨까요.

<english>
Analysis on the result when train model to reason using SFT. For easy problems performance increases greatly with small number of samples, but hard problems requires a lot more samples. What would be pattern when RL is used.
</english>

#reasoning 