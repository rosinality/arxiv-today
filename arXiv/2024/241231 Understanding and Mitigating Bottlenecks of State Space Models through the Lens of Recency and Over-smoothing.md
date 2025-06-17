https://arxiv.org/abs/2501.00658

*Understanding and Mitigating Bottlenecks of State Space Models through the Lens of Recency and Over-smoothing* (Peihao Wang, Ruisi Cai, Yuehao Wang, Jiajun Zhu, Pragya Srivastava, Zhangyang Wang, Pan Li)

> Structured State Space Models (SSMs) have emerged as alternatives to transformers. While SSMs are often regarded as effective in capturing long-sequence dependencies, we rigorously demonstrate that they are inherently limited by strong recency bias. Our empirical studies also reveal that this bias impairs the models' ability to recall distant information and introduces robustness issues. Our scaling experiments then discovered that deeper structures in SSMs can facilitate the learning of long contexts. However, subsequent theoretical analysis reveals that as SSMs increase in depth, they exhibit another inevitable tendency toward over-smoothing, e.g., token representations becoming increasingly indistinguishable. This fundamental dilemma between recency and over-smoothing hinders the scalability of existing SSMs. Inspired by our theoretical findings, we propose to polarize two channels of the state transition matrices in SSMs, setting them to zero and one, respectively, simultaneously addressing recency bias and over-smoothing. Experiments demonstrate that our polarization technique consistently enhances the associative recall accuracy of long-range tokens and unlocks SSMs to benefit further from deeper architectures. All source codes are released at https://github.com/VITA-Group/SSM-Bottleneck.

State Space Model의 Time decay로 인한 Long range dependency 모델링에서의 한계, 그리고 그것을 해결하기 위해 레이어를 쌓았을 때 SSM이 Low pass filter라는 것에 의해 발생하는 Over smoothing, 즉 토큰 임베딩이 서로 비슷해지는 문제에 대한 분석.

이에 대해 Transition 행렬의 최대/최소를 1과 0으로 고정하기 위해 일부를 상수로 고정해버리는 방법을 시도했네요.

<english>
Limitation of state space models on long range dependency modelings due to time decay. And analysis on over-smoothing problems which is token embeddings became similar because of SSM is low pass filter, that occurs when we stacks more layer to model long range dependency.

For this problem they tried to partially set a value of transition matrix to 0 and 1 to fix maximum and minimum of it to be 1 and 0.
</english>

#state-space-model 