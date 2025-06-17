https://arxiv.org/abs/2503.04548

*An Empirical Study on Eliciting and Improving R1-like Reasoning Models* (Zhipeng Chen, Yingqian Min, Beichen Zhang, Jie Chen, Jinhao Jiang, Daixuan Cheng, Wayne Xin Zhao, Zheng Liu, Xu Miao, Yang Lu, Lei Fang, Zhongyuan Wang, Ji-Rong Wen)

> In this report, we present the third technical report on the development of slow-thinking models as part of the STILL project. As the technical pathway becomes clearer, scaling RL training has become a central technique for implementing such reasoning models. We systematically experiment with and document the effects of various factors influencing RL training, conducting experiments on both base models and fine-tuned models. Specifically, we demonstrate that our RL training approach consistently improves the Qwen2.5-32B base models, enhancing both response length and test accuracy. Furthermore, we show that even when a model like DeepSeek-R1-Distill-Qwen-1.5B has already achieved a high performance level, it can be further refined through RL training, reaching an accuracy of 39.33% on AIME 2024. Beyond RL training, we also explore the use of tool manipulation, finding that it significantly boosts the reasoning performance of large reasoning models. This approach achieves a remarkable accuracy of 86.67% with greedy search on AIME 2024, underscoring its effectiveness in enhancing model capabilities. We release our resources at the STILL project website: https://github.com/RUCAIBox/Slow_Thinking_with_LLMs.

추론 RL에 어떻게 접근해야 하는지가 알려지니 모두들 실험하고 리포트를 작성하고 있네요. 그래서 방향을 제시하는 것, 그리고 그 방향으로 어떻게 나아가야 하는지를 알아내는 것이 무엇보다 더 영향력 있는 일인 것이겠죠.

<english>
After the way to approach reasoning RL is disclosed, now everyone doing experiments and writing a report. Thus suggesting directions, and find out how we should progress in that direction is most influential thing to do.
</english>

#reasoning #rl 