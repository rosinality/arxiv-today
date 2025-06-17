https://github.com/ruixin31/Rethink_RLVR/blob/main/paper/rethink-rlvr.pdf

**Spurious Rewards: Rethinking Training Signals in RLVR** (Rulin Shao, Shuyue Stella Li, Rui Xin, Scott Geng, Yiping Wang, Sewoong Oh, Simon Shaolei Du, Nathan Lambert, Sewon Min, Ranjay Krishna, Yulia Tsvetkov, Hannaneh Hajishirzi, Pang Wei Koh, Luke Zettlemoyer)

> We show that reinforcement learning with verifiable rewards (RLVR) can elicit strong mathematical reasoning in certain models even with spurious rewards that have little, no, or even negative correlation with the correct answer. For example, RLVR improves MATH-500 performance for Qwen2.5-Math-7B in absolute points by 21.4% (random reward), 16.4% (format reward), 24.6% (incorrect label), 24.4% (1-shot RL), and 26.5% (majority voting)—nearly matching the 28.8% gained with ground truth rewards. However, the spurious rewards that work for Qwen often fail to yield gains with other model families like Llama3 or OLMo2. In particular, we find code reasoning—thinking in code without actual code execution—to be a distinctive Qwen2.5-Math behavior that becomes significantly more frequent after RLVR, from 66.7% to over 90%, even with spurious rewards. Overall, we hypothesize that, given the lack of useful reward signal, RLVR must somehow be surfacing useful reasoning representations learned during pretraining, although the exact mechanism remains a topic for future work. We suggest that future RLVR research should possibly be validated on diverse models rather than a single de facto choice, as we show that it is easy to get significant performance gains on Qwen models even with completely spurious reward signals.

랜덤이나 잘못된 정답 기반으로 Reward를 주어도 추론 RL 학습이 가능하다는 발견. 단, Qwen에서만. Qwen은 이전부터 Instruction 데이터가 많이 들어갔고 추론 미드트레이닝까지 하고 있으니 좀 이질적인 모델이죠. Qwen으로만 실험한 추론 RL이 "쉽게" 된다는 연구들은 앞으로 주의해야 한다는 결과네요.

<english>
Discovery of it is possible to do reasoning RL training with incorrect or random rewards. But, only with Qwen. Qwen traditionally used a lot of instruction data and as nowadays incorporates reasoning mid-training it is somewhat different class of models. It would mean that we should cautious about the result insist that reasoning RL is "easy" only with experiments on Qwen.
</english>

#reasoning #rl 