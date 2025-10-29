https://arxiv.org/abs/2510.24397

*APTBench: Benchmarking Agentic Potential of Base LLMs During Pre-Training* (Jiarui Qin, Yunjia Xi, Junjie Huang, Renting Rui, Di Yin, Weiwen Liu, Yong Yu, Weinan Zhang, Xing Sun)

> With the rapid development of LLM-based agents, there is a growing trend to incorporate agent-specific data into the pre-training stage of LLMs, aiming to better align LLMs with real-world autonomous task execution. However, current pre-training benchmarks primarily focus on isolated and static skills, e.g., common knowledge or mathematical/code reasoning, and fail to reflect model's agentic capabilities. On the other hand, agent benchmarks are typically designed for post-trained models, requiring multi-turn task execution abilities that base models struggle to support. Thus, there is a compelling need for a benchmark that can evaluate agentic potentials during pre-training and guide the model training more effectively. To address this gap, we propose APTBench, a framework that converts real-world agent tasks and successful trajectories into multiple-choice or text completion questions tailored for base models. It focuses on core agentic abilities, e.g., planning and action, and covers key agent scenarios, software engineering and deep research. Compared to existing general-purpose benchmarks, APTBench offers a more predictive signal of a model's downstream performance as an agent, while remaining significantly more lightweight and cost-effective than full-scale, end-to-end agent evaluations after post-training.

프리트레이닝된 베이스 모델의 에이전트 능력을 평가. 에이전틱 궤적을 생성하고 텍스트 완성이나 객관식 문제를 만들어 계획이나 액션 선택 능력을 측정.

Evaluate agentic capabilities of pretrained base model. Built agentic trajectories and made text completion or multiple choice questions from them to measure planning or action abilities.

#benchmark #agent 