https://arxiv.org/abs/2309.06657

Statistical Rejection Sampling Improves Preference Optimization (Tianqi Liu, Yao Zhao, Rishabh Joshi, Misha Khalman, Mohammad Saleh, Peter J. Liu, Jialu Liu)

Direct Preference Optimization (https://arxiv.org/abs/2305.18290) 과 SLiC-HF (https://arxiv.org/abs/2305.10425) 을 분석해서 개선한 방법이군요.

1. DPO. DPO는 학습 중인 policy에서 나온 샘플이 아니라 어떤 다른 policy에서 샘플링한 결과에 대한 preference label을 사용하는 방법이죠.
2. SLiC-HF (sample-rank variant)는 학습 중인 policy를 사용해서 샘플링한 다음, reward model로 preference label을 부여해서 학습하는 방법입니다.
3. 제안된 방법 RSO는 reward에 대해 optimal한 policy를 사용해서 샘플링한 다음, reward model로 preference label을 부여해서 학습하는 방법입니다.

차이는 optimal policy를 사용하는가에 있는 것 같고 (optimal policy가 목표이기 때문에 optimal policy에서 나온 샘플을 쓰는 것이 좋다는 아이디어입니다.) 그러면 optimal policy에서 샘플링을 어떻게 할 것인가? rejection sampling을 사용합니다.

흥미롭네요. DPO와 SLiC-HF보다 나은 결과를 보고하고 있습니다. 그러나 PPO와 비교하면 어떨까요. 그 결과가 없긴 하네요.

[[230529 Direct Preference Optimization]]
[[230517 SLiC-HF]]
[[230817 Reinforced Self-Training (ReST) for Language Modeling]]

#alignment #rl

# Links

[[230529 Direct Preference Optimization.md]]
[[230517 SLiC-HF.md]]