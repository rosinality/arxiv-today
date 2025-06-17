https://arxiv.org/abs/2502.12272

*Learning to Reason at the Frontier of Learnability* (Thomas Foster, Jakob Foerster)

> Reinforcement learning is now widely adopted as the final stage of large language model training, especially for reasoning-style tasks such as maths problems. Typically, models attempt each question many times during a single training step and attempt to learn from their successes and failures. However, we demonstrate that throughout training with two popular algorithms (PPO and VinePPO) on two widely used datasets, many questions are either solved by all attempts - meaning they are already learned - or by none - providing no meaningful training signal. To address this, we adapt a method from the reinforcement learning literature - sampling for learnability - and apply it to the reinforcement learning stage of LLM training. Our curriculum prioritises questions with high variance of success, i.e. those where the agent sometimes succeeds, but not always. Our findings demonstrate that this curriculum consistently boosts training performance across multiple algorithms and datasets, paving the way for more efficient and effective reinforcement learning in LLMs.

정답률 p를 사용한 Learnability p(1 - p)를 사용해 추론 RL을 진행. 이런 커리큘럼을 만드는 방법들이 자연스럽게 등장하고 있네요. (https://arxiv.org/abs/2502.11886)

<english>
Doing reasoning RL using learnability p(1 - p), where p is rate of correct answers. A method for building curriculum like this now appearing naturally. (https://arxiv.org/abs/2502.11886)
</english>

#rl #reasoning 