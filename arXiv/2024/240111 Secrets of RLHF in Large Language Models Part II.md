https://arxiv.org/abs/2401.06080

*Secrets of RLHF in Large Language Models Part II: Reward Modeling* (Binghai Wang, Rui Zheng, Lu Chen, Yan Liu, Shihan Dou, Caishuang Huang, Wei Shen, Senjie Jin, Enyu Zhou, Chenyu Shi, Songyang Gao, Nuo Xu, Yuhao Zhou, Xiaoran Fan, Zhiheng Xi, Jun Zhao, Xiao Wang, Tao Ji, Hang Yan, Lixing Shen, Zhan Chen, Tao Gui, Qi Zhang, Xipeng Qiu, Xuanjing Huang, Zuxuan Wu, Yu-Gang Jiang)

> Reinforcement Learning from Human Feedback (RLHF) has become a crucial technology for aligning language models with human values and intentions, enabling models to produce more helpful and harmless responses. Reward models are trained as proxies for human preferences to drive reinforcement learning optimization. While reward models are often considered central to achieving high performance, they face the following challenges in practical applications: (1) Incorrect and ambiguous preference pairs in the dataset may hinder the reward model from accurately capturing human intent. (2) Reward models trained on data from a specific distribution often struggle to generalize to examples outside that distribution and are not suitable for iterative RLHF training. In this report, we attempt to address these two issues. (1) From a data perspective, we propose a method to measure the strength of preferences within the data, based on a voting mechanism of multiple reward models. Experimental results confirm that data with varying preference strengths have different impacts on reward model performance. We introduce a series of novel methods to mitigate the influence of incorrect and ambiguous preferences in the dataset and fully leverage high-quality preference data. (2) From an algorithmic standpoint, we introduce contrastive learning to enhance the ability of reward models to distinguish between chosen and rejected responses, thereby improving model generalization. Furthermore, we employ meta-learning to enable the reward model to maintain the ability to differentiate subtle differences in out-of-distribution samples, and this approach can be utilized for iterative RLHF optimization.

드디어 https://arxiv.org/abs/2307.04964 의 파트 2가 나왔군요. Reward Model 앙상블 쪽에서 나온 결과들의 연장선상에서 모델들의 스코어 차이로 Preference 데이터의 노이즈를 찾아내는 것에서 시작합니다. 이 노이즈에 대한 대응으로 Label smoothing, Label flipping 같은 다소 전통적인(?) Overconfidence 대책들과 Llama 2의 Margin을 시도해봤네요.

추가로 Positive vs Negative의 차이를 증가시키기 위한 Contrastive objective와 PPO 학습 과정에서의 distribution shift에 대응하는 메타 러닝을 실험했습니다. 모두 굉장히 흥미로운 주제네요. Weak to strong generalization에도 관련지어 생각해볼 수 있지 않을까 싶습니다.

#rlhf

# Links

[[230711 Secrets of RLHF in Large Language Models Part I.md]]