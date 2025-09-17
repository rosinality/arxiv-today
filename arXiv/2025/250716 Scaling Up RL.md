https://arxiv.org/abs/2507.12507

*Scaling Up RL: Unlocking Diverse Reasoning in LLMs via Prolonged Training* (Mingjie Liu, Shizhe Diao, Jian Hu, Ximing Lu, Xin Dong, Hao Zhang, Alexander Bukharin, Shaokun Zhang, Jiaqi Zeng, Makesh Narsimhan Sreedhar, Gerald Shen, David Mosallanezhad, Di Zhang, Jonas Yang, June Yang, Oleksii Kuchaiev, Guilin Liu, Zhiding Yu, Pavlo Molchanov, Yejin Choi, Jan Kautz, Yi Dong)

> Recent advancements in reasoning-focused language models such as OpenAI's O1 and DeepSeek-R1 have shown that scaling test-time computation-through chain-of-thought reasoning and iterative exploration-can yield substantial improvements on complex tasks like mathematics and code generation. These breakthroughs have been driven by large-scale reinforcement learning (RL), particularly when combined with verifiable reward signals that provide objective and grounded supervision. In this report, we investigate the effects of prolonged reinforcement learning on a small language model across a diverse set of reasoning domains. Our work identifies several key ingredients for effective training, including the use of verifiable reward tasks, enhancements to Group Relative Policy Optimization (GRPO), and practical techniques to improve training stability and generalization. We introduce controlled KL regularization, clipping ratio, and periodic reference policy resets as critical components for unlocking long-term performance gains. Our model achieves significant improvements over strong baselines, including +14.7% on math, +13.9% on coding, and +54.8% on logic puzzle tasks. To facilitate continued research, we release our model publicly.

NVIDIA의 추론 RL 실험. 1.5B 모델로 실험했군요. 제목도 그렇고 ProRL과 비슷하네요 (https://arxiv.org/abs/2505.24864).

<english>
NVIDIA's experiment on reasoning RL. Based on 1.5B models. Like title it is quite similar to ProRL (https://arxiv.org/abs/2505.24864).
</english>

#rl #reasoning 