https://arxiv.org/abs/2402.08939

*Premise Order Matters in Reasoning with Large Language Models* (Xinyun Chen, Ryan A. Chi, Xuezhi Wang, Denny Zhou)

> Large language models (LLMs) have accomplished remarkable reasoning performance in various domains. However, in the domain of reasoning tasks, we discover a frailty: LLMs are surprisingly brittle to the ordering of the premises, despite the fact that such ordering does not alter the underlying task. In particular, we observe that LLMs achieve the best performance when the premise order aligns with the context required in intermediate reasoning steps. For example, in deductive reasoning tasks, presenting the premises in the same order as the ground truth proof in the prompt (as opposed to random ordering) drastically increases the model's accuracy. We first examine the effect of premise ordering on deductive reasoning on a variety of LLMs, and our evaluation shows that permuting the premise order can cause a performance drop of over 30%. In addition, we release the benchmark R-GSM, based on GSM8K, to examine the ordering effect for mathematical problem-solving, and we again observe a significant drop in accuracy, relative to the original GSM8K benchmark.

전제의 순서가 바뀌면 LLM의 추론 성능이 바뀐다는 결과. 즉 A -> B, B -> C 순서일 때가 B -> C, A -> B 순서일 때보다 성능이 낫다는 것이네요. Reversal Curse (https://arxiv.org/abs/2309.12288) 가 떠오르네요.

#llm

# Links

[[230921 The Reversal Curse.md]]