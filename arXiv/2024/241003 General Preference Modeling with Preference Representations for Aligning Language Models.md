https://arxiv.org/abs/2410.02197

*General Preference Modeling with Preference Representations for Aligning Language Models* (Yifan Zhang, Ge Zhang, Yue Wu, Kangping Xu, Quanquan Gu)

> Modeling human preferences is crucial for aligning foundation models with human values. Traditional reward modeling methods, such as the Bradley-Terry (BT) reward model, fall short in expressiveness, particularly in addressing intransitive preferences. Although supervised pair preference models (PairPM) can express general preferences, their implementation is highly ad-hoc and cannot guarantee a consistent preference probability of compared pairs. Additionally, they impose high computational costs due to their quadratic query complexity when comparing multiple responses. In this paper, we introduce preference representation learning, an approach that embeds responses into a latent space to capture intricate preference structures efficiently, achieving linear query complexity. Additionally, we propose preference score-based General Preference Optimization (GPO), which generalizes reward-based reinforcement learning from human feedback. Experimental results show that our General Preference representation model (GPM) outperforms the BT reward model on the RewardBench benchmark with a margin of up to 5.6% and effectively models cyclic preferences where any BT reward model behaves like a random guess. Furthermore, evaluations on downstream tasks such as AlpacaEval2.0 and MT-Bench, following the language model post-training with GPO and our general preference model, reveal substantial performance improvements with margins up to 9.3%. These findings indicate that our method may enhance the alignment of foundation models with nuanced human values. The code is available at https://github.com/general-preference/general-preference-model.

여러 응답에 대해서 선호의 Intransitivity를 모델링하기 위한 방법. 각 응답에 대한 임베딩 벡터를 추출한 다음 Skew-symmetric Operator를 사용해 스코어를 계산합니다.

<english>
Modeling intransitivity of preferences among multiple responses. Extracting embedding vectors from each responses and calculate scores using skew-symmetric operator.
</english>

#rlhf #reward-model 