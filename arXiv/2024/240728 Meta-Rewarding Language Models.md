https://arxiv.org/abs/2407.19594

*Meta-Rewarding Language Models: Self-Improving Alignment with LLM-as-a-Meta-Judge* (Tianhao Wu, Weizhe Yuan, Olga Golovneva, Jing Xu, Yuandong Tian, Jiantao Jiao, Jason Weston, Sainbayar Sukhbaatar)

> Large Language Models (LLMs) are rapidly surpassing human knowledge in many domains. While improving these models traditionally relies on costly human data, recent self-rewarding mechanisms (Yuan et al., 2024) have shown that LLMs can improve by judging their own responses instead of relying on human labelers. However, existing methods have primarily focused on improving model responses rather than judgment capabilities, resulting in rapid saturation during iterative training. To address this issue, we introduce a novel Meta-Rewarding step to the self-improvement process, where the model judges its own judgements and uses that feedback to refine its judgment skills. Surprisingly, this unsupervised approach improves the model's ability to judge {\em and} follow instructions, as demonstrated by a win rate improvement of Llama-3-8B-Instruct from 22.9% to 39.4% on AlpacaEval 2, and 20.6% to 29.1% on Arena-Hard. These results strongly suggest the potential for self-improving models without human supervision.

Self-rewarding처럼 (https://arxiv.org/abs/2401.10020) 모델 하나에 Actor와 Judge의 역할을 부여해 Actor의 생성 결과를 Judge로 분류해 학습시키는 방법에서, 추가적으로 Judge를 학습시키기 위해 Judge의 결과를 분류하는 Meta Judge 역할을 추가한 방법.

#rlaif #synthetic-data

# Links

[[240118 Self-Rewarding Language Models.md]]