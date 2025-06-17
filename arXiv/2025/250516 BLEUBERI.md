https://arxiv.org/abs/2505.11080

*BLEUBERI: BLEU is a surprisingly effective reward for instruction following* (Yapei Chang, Yekyung Kim, Michael Krumdick, Amir Zadeh, Chuan Li, Chris Tanner, Mohit Iyyer)

> Reward models are central to aligning LLMs with human preferences, but they are costly to train, requiring large-scale human-labeled preference data and powerful pretrained LLM backbones. Meanwhile, the increasing availability of high-quality synthetic instruction-following datasets raises the question: can simpler, reference-based metrics serve as viable alternatives to reward models during RL-based alignment? In this paper, we show first that BLEU, a basic string-matching metric, surprisingly matches strong reward models in agreement with human preferences on general instruction-following datasets. Based on this insight, we develop BLEUBERI, a method that first identifies challenging instructions and then applies Group Relative Policy Optimization (GRPO) using BLEU directly as the reward function. We demonstrate that BLEUBERI-trained models are competitive with models trained via reward model-guided RL across four challenging instruction-following benchmarks and three different base language models. A human evaluation further supports that the quality of BLEUBERI model outputs is on par with those from reward model-aligned models. Moreover, BLEUBERI models generate outputs that are more factually grounded than competing methods. Overall, we show that given access to high-quality reference outputs (easily obtained via existing instruction-following datasets or synthetic data generation), string matching-based metrics are cheap yet effective proxies for reward models during alignment. We release our code and data at https://github.com/lilakk/BLEUBERI.

BLEU로 Instruction Following에 대한 Reward를 줄 수 있다는 연구. 조금 다른 이야기지만 WorldPM에서 (https://arxiv.org/pdf/2505.11080) 규칙 기반 Reward와 Retrieval, Generative Matching 등이 존재할 때 Reward Model의 역할은 무엇인가라는 질문을 하더군요. 흥미로운 지점이라고 봅니다.

<english>
The study suggests that it is possible to assign reward for insturction following using BLEU. Though slightly different idea, but WorldPM discusses about the role of reward models when rule-based rewards, retrieval or generative matching rewards. I think it is interesting point.
</english>

#reward-model #alignment 