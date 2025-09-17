https://arxiv.org/abs/2509.06160

*Reverse-Engineered Reasoning for Open-Ended Generation* (Haozhe Wang, Haoran Que, Qixin Xu, Minghao Liu, Wangchunshu Zhou, Jiazhan Feng, Wanjun Zhong, Wei Ye, Tong Yang, Wenhao Huang, Ge Zhang, Fangzhen Lin)

> While the ``deep reasoning'' paradigm has spurred significant advances in verifiable domains like mathematics, its application to open-ended, creative generation remains a critical challenge. The two dominant methods for instilling reasoning -- reinforcement learning (RL) and instruction distillation -- falter in this area; RL struggles with the absence of clear reward signals and high-quality reward models, while distillation is prohibitively expensive and capped by the teacher model's capabilities. To overcome these limitations, we introduce REverse-Engineered Reasoning (REER), a new paradigm that fundamentally shifts the approach. Instead of building a reasoning process ``forwards'' through trial-and-error or imitation, REER works ``backwards'' from known-good solutions to computationally discover the latent, step-by-step deep reasoning process that could have produced them. Using this scalable, gradient-free approach, we curate and open-source DeepWriting-20K, a large-scale dataset of 20,000 deep reasoning trajectories for open-ended tasks. Our model, DeepWriter-8B, trained on this data, not only surpasses strong open-source baselines but also achieves performance competitive with, and at times superior to, leading proprietary models like GPT-4o and Claude 3.5.

Open-ended 응답에 대한 추론 궤적을 레퍼런스 데이터에서 찾아내기. Reward로는 추론에 대한 응답의 Perplexity를 사용. 그리고 초기 궤적의 각 부분을 개선하는 방법으로 추론 궤적을 탐색.

Searching for reasoning trajectories for open-ended responses from reference answers. As a reward perplexity of responses given the reasoning is used. The reasoning trajectories are explored by improving each segment of the initial trajectories.

#post-training #reasoning 