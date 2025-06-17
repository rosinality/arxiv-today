https://arxiv.org/abs/2402.16030

*Don't Forget Your Reward Values: Language Model Alignment via Value-based Calibration* (Xin Mao, Feng-Lin Li, Huimin Xu, Wei Zhang, Anh Tuan Luu)

> While Reinforcement Learning from Human Feedback (RLHF) significantly enhances the generation quality of Large Language Models (LLMs), recent studies have raised concerns regarding the complexity and instability associated with the Proximal Policy Optimization (PPO) algorithm, proposing a series of order-based calibration methods as viable alternatives. This paper delves further into current order-based methods, examining their inefficiencies in utilizing reward values and addressing misalignment issues. Building upon these findings, we propose a novel \textbf{V}alue-based \textbf{C}ali\textbf{B}ration (VCB) method to better align LLMs with human preferences. Experimental results demonstrate that VCB surpasses existing alignment methods on AI assistant and summarization datasets, providing impressive generalizability, robustness, and stability in diverse settings.

N개 샘플을 뽑고 Reward Model로 계산한 스코어를 사용한다는 아이디어는 계속되는군요. DPO 식의 Likelihood의 차이가 표준편차로 정규화된 Reward Score의 차이와 같게 튜닝하는 형태입니다.

#rlhf 