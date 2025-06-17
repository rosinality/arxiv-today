https://arxiv.org/abs/2402.07610

*Step-On-Feet Tuning: Scaling Self-Alignment of LLMs via Bootstrapping* (Haoyu Wang, Guozheng Ma, Ziqiao Meng, Zeyu Qin, Li Shen, Zhong Zhang, Bingzhe Wu, Liu Liu, Yatao Bian, Tingyang Xu, Xueqian Wang, Peilin Zhao)

> Self-alignment is an effective way to reduce the cost of human annotation while ensuring promising model capability. However, most current methods complete the data collection and training steps in a single round, which may overlook the continuously improving ability of self-aligned models. This gives rise to a key query: What if we do multi-time bootstrapping self-alignment? Does this strategy enhance model performance or lead to rapid degradation? In this paper, our pioneering exploration delves into the impact of bootstrapping self-alignment on large language models. Our findings reveal that bootstrapping self-alignment markedly surpasses the single-round approach, by guaranteeing data diversity from in-context learning. To further exploit the capabilities of bootstrapping, we investigate and adjust the training order of data, which yields improved performance of the model. Drawing on these findings, we propose Step-On-Feet Tuning (SOFT) which leverages model's continuously enhanced few-shot ability to boost zero or one-shot performance. Based on easy-to-hard training recipe, we propose SOFT+ which further boost self-alignment's performance. Our experiments demonstrate the efficiency of SOFT (SOFT+) across various classification and generation tasks, highlighting the potential of bootstrapping self-alignment on continually enhancing model alignment performance.

Dromedary (https://arxiv.org/abs/2305.03047) 계통의 방법이군요. SFT를 통해 Instruction Following 능력이 향상된다면, 프리트레이닝된 모델로 SFT를 한 번 하는 것이 아니라 데이터셋을 쪼개 살짝 튜닝된 모델로 다시 응답을 만들어 학습시키는 것이 낫지 않을까 하는 생각입니다.

#instruction-tuning #synthetic-data 

This paper suggests self alignment method in the lineage of Dromedary. If we can expect instruction following ability of the model is enhanced during SFT, then it could be better to split datasets and using generated responses from model trained on subset datasets could be better than doing SFT on pretrained model once.

# Links

[[230504 Principle-Driven Self-Alignment of Language Models from Scratch with Minimal Human Supervision.md]]