https://arxiv.org/abs/2503.22230

*Exploring Data Scaling Trends and Effects in Reinforcement Learning from Human Feedback* (Wei Shen, Guanlin Liu, Zheng Wu, Ruofei Zhu, Qingping Yang, Chao Xin, Yu Yue, Lin Yan)

> Reinforcement Learning from Human Feedback (RLHF) is crucial for aligning large language models with human preferences. While recent research has focused on algorithmic improvements, the importance of prompt-data construction has been overlooked. This paper addresses this gap by exploring data-driven bottlenecks in RLHF performance scaling, particularly reward hacking and decreasing response diversity. We introduce a hybrid reward system combining reasoning task verifiers (RTV) and a generative reward model (GenRM) to mitigate reward hacking. We also propose a novel prompt-selection method, Pre-PPO, to maintain response diversity and enhance learning effectiveness. Additionally, we find that prioritizing mathematical and coding tasks early in RLHF training significantly improves performance. Experiments across two model sizes validate our methods' effectiveness and scalability. Results show that RTV is most resistant to reward hacking, followed by GenRM with ground truth, and then GenRM with SFT Best-of-N responses. Our strategies enable rapid capture of subtle task-specific distinctions, leading to substantial improvements in overall RLHF performance. This work highlights the importance of careful data construction and provides practical methods to overcome performance barriers in RLHF.

RLHF 과정의 Reward Hacking과 다양성 감소에 대한 대응. Verifiable Reward와 GT를 사용하는 Reward Model을 추가로 사용, Reward Score가 낮은 프롬프트를 선택, 그리고 수학과 코딩에 대해서 먼저 학습시키는 전략을 사용했군요.

<english>
Resolution on reward hacking and decrease of diversity during RLHF. The strategy is using additional verifiable reward and reward model that utilizes ground truth, selecting prompt with low reward scores, and training in math and coding domains in early stage of the training.
</english>

#rlhf #reward-model 