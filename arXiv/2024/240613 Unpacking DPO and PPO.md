https://arxiv.org/abs/2406.09279

*Unpacking DPO and PPO: Disentangling Best Practices for Learning from Preference Feedback* (Hamish Ivison, Yizhong Wang, Jiacheng Liu, Zeqiu Wu, Valentina Pyatkin, Nathan Lambert, Noah A. Smith, Yejin Choi, Hannaneh Hajishirzi)

> Learning from preference feedback has emerged as an essential step for improving the generation quality and performance of modern language models (LMs). Despite its widespread use, the way preference-based learning is applied varies wildly, with differing data, learning algorithms, and evaluations used, making disentangling the impact of each aspect difficult. In this work, we identify four core aspects of preference-based learning: preference data, learning algorithm, reward model, and policy training prompts, systematically investigate the impact of these components on downstream model performance, and suggest a recipe for strong learning for preference feedback. Our findings indicate that all aspects are important for performance, with better preference data leading to the largest improvements, followed by the choice of learning algorithm, the use of improved reward models, and finally the use of additional unlabeled prompts for policy training. Notably, PPO outperforms DPO by up to 2.5% in math and 1.2% in general domains. High-quality preference data leads to improvements of up to 8% in instruction following and truthfulness. Despite significant gains of up to 5% in mathematical evaluation when scaling up reward models, we surprisingly observe marginal improvements in other categories. We publicly release the code used for training (https://github.com/hamishivi/EasyLM) and evaluating (https://github.com/allenai/open-instruct) our models, along with the models and datasets themselves (https://huggingface.co/collections/allenai/tulu-v25-suite-66676520fd578080e126f618).

LLM의 RL 과정의 요인들의 효과 평가. 데이터셋 퀄리티가 중요하고, PPO > DPO이고, Reward Model이 강력하면 좋겠지만 Reward Bench 스코어가 성능으로 이어지는 것은 아니고, PPO 과정에서 레이블은 없더라도 타겟 도메인에 대한 프롬프트를 사용할 수 있으면 좋다는 결과. PPO + 프롬프트 증폭은 Anthropic이 (https://arxiv.org/abs/2204.05862) 사용해왔던 트릭이기도 하죠.

데이터를 잘 만들고 방법에 집착하지 않을 것. ML 업계의 오래된 교훈이지만 그만큼 어려운 것인 것 같기도 합니다.

#alignment

# Links

[[230629 Training a Helpful and Harmless Assistant with Reinforcement Learning from Human Feedback.md]]