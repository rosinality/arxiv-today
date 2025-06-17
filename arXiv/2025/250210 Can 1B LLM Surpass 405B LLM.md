https://arxiv.org/abs/2502.06703

*Can 1B LLM Surpass 405B LLM? Rethinking Compute-Optimal Test-Time Scaling* (Runze Liu, Junqi Gao, Jian Zhao, Kaiyan Zhang, Xiu Li, Biqing Qi, Wanli Ouyang, Bowen Zhou)

> Test-Time Scaling (TTS) is an important method for improving the performance of Large Language Models (LLMs) by using additional computation during the inference phase. However, current studies do not systematically analyze how policy models, Process Reward Models (PRMs), and problem difficulty influence TTS. This lack of analysis limits the understanding and practical use of TTS methods. In this paper, we focus on two core questions: (1) What is the optimal approach to scale test-time computation across different policy models, PRMs, and problem difficulty levels? (2) To what extent can extended computation improve the performance of LLMs on complex tasks, and can smaller language models outperform larger ones through this approach? Through comprehensive experiments on MATH-500 and challenging AIME24 tasks, we have the following observations: (1) The compute-optimal TTS strategy is highly dependent on the choice of policy model, PRM, and problem difficulty. (2) With our compute-optimal TTS strategy, extremely small policy models can outperform larger models. For example, a 1B LLM can exceed a 405B LLM on MATH-500. Moreover, on both MATH-500 and AIME24, a 0.5B LLM outperforms GPT-4o, a 3B LLM surpasses a 405B LLM, and a 7B LLM beats o1 and DeepSeek-R1, while with higher inference efficiency. These findings show the significance of adapting TTS strategies to the specific characteristics of each task and model and indicate that TTS is a promising approach for enhancing the reasoning abilities of LLMs.

PRM과 탐색을 사용한 최적 Inference-time Scaling 방법 탐색. PRM이 일반화가 잘 되지 않는다는 문제를 여기서도 지적하고 있고, 이 일반화 문제 때문에 최적 탐색 전략 또한 PRM에 따라 변화하는군요.

<english>
Analysis on compute optimal inference-time scaling using PRM and search. They also points out PRM does not generalizes well, and this generalization problems makes optimal exploration strategy to be changed per PRM.
</english>

#inference-time-scaling #reward-model 