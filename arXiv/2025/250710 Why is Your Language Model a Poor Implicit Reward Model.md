https://arxiv.org/abs/2507.07981

*Why is Your Language Model a Poor Implicit Reward Model?* (Noam Razin, Yong Lin, Jiarui Yao, Sanjeev Arora)

> Reward models are key to language model post-training and inference pipelines. Conveniently, recent work showed that every language model defines an implicit reward model (IM-RM), without requiring any architectural changes. However, such IM-RMs tend to generalize worse, especially out-of-distribution, compared to explicit reward models (EX-RMs) that apply a dedicated linear head over the hidden representations of a language model. The existence of a generalization gap is puzzling, as EX-RMs and IM-RMs are nearly identical. They can be trained using the same data, loss function, and language model, and differ only in how the reward is computed. Towards a fundamental understanding of the implicit biases underlying different reward model types, we investigate the root cause of this gap. Our main finding, backed by theory and experiments, is that IM-RMs rely more heavily on superficial token-level cues. Consequently, they often generalize worse than EX-RMs under token-level distribution shifts, as well as in-distribution. Furthermore, we provide evidence against alternative hypotheses for the generalization gap. Most notably, we challenge the intuitive claim that IM-RMs struggle in tasks where generation is harder than verification because they can operate both as a verifier and a generator. Taken together, our results highlight that seemingly minor design choices can substantially impact the generalization behavior of reward models.

Implicit Reward로 Parameterization 하는 것이 명시적인 Reward 헤드보다 일반화 성능이 떨어지는 문제에 대한 분석. Implicit Reward의 경우에 토큰 단위 단서를 활용하는 경향이 크다고 하네요.

<english>
An analysis on the problem of decrease in generalization when reward model is parameterized as implicit reward compared to using explit reward heads. The authors insist that implicit rewards relies more on token level cues.
</english>

#reward-model #generalization 