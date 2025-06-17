https://arxiv.org/abs/2412.18279

*Improving Multi-Step Reasoning Abilities of Large Language Models with Direct Advantage Policy Optimization* (Jiacai Liu, Chaojie Wang, Chris Yuhao Liu, Liang Zeng, Rui Yan, Yiwen Sun, Yang Liu, Yahui Zhou)

> The role of reinforcement learning (RL) in enhancing the reasoning of large language models (LLMs) is becoming increasingly significant. Despite the success of RL in many scenarios, there are still many challenges in improving the reasoning of LLMs. One challenge is the sparse reward, which makes optimization difficult for RL and necessitates a large amount of data samples. Another challenge stems from the inherent instability of RL, particularly when using Actor-Critic (AC) methods to derive optimal policies, which often leads to unstable training processes. To address these issues, we introduce Direct Advantage Policy Optimization (DAPO), an novel step-level offline RL algorithm. Unlike standard alignment that rely solely outcome rewards to optimize policies (such as DPO), DAPO employs a critic function to predict the reasoning accuracy at each step, thereby generating dense signals to refine the generation strategy. Additionally, the Actor and Critic components in DAPO are trained independently, avoiding the co-training instability observed in standard AC algorithms like PPO. We train DAPO on mathematical and code query datasets and then evaluate its performance on multiple benchmarks. Our results show that DAPO can effectively enhance the mathematical and code capabilities on both SFT models and RL models, demonstrating the effectiveness of DAPO.

따로 학습한 Critic을 사용하는 오프라인 RL. Critic 학습에서 Generator와 Completer를 구분해 Generator로 추론 단계를 생성한 다음 Completer로 나머지 단계를 생성하고 정답과 비교하는 형태로 Value를 추정하는 방법을 사용했네요.

<english>
Offline RL method that employs critic trained in separately. During training the critic they distinguishes generator and critic, and they estimated value by samples reasoning step using generator and rest of that trajectory by completer then compares with the answer.
</english>

#reasoning #rl 