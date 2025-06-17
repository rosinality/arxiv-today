https://arxiv.org/abs/2412.02674

*Mind the Gap: Examining the Self-Improvement Capabilities of Large Language Models* (Yuda Song, Hanlin Zhang, Carson Eisenach, Sham Kakade, Dean Foster, Udaya Ghai)

> Self-improvement is a mechanism in Large Language Model (LLM) pre-training, post-training and test-time inference. We explore a framework where the model verifies its own outputs, filters or reweights data based on this verification, and distills the filtered data. Despite several empirical successes, a fundamental understanding is still lacking. In this work, we initiate a comprehensive, modular and controlled study on LLM self-improvement. We provide a mathematical formulation for self-improvement, which is largely governed by a quantity which we formalize as the generation-verification gap. Through experiments with various model families and tasks, we discover a scaling phenomenon of self-improvement -- a variant of the generation-verification gap scales monotonically with the model pre-training flops. We also examine when self-improvement is possible, an iterative self-improvement procedure, and ways to improve its performance. Our findings not only advance understanding of LLM self-improvement with practical implications, but also open numerous avenues for future research into its capabilities and boundaries.

Self Improvement이 가능한 것은 Generation과 Verification에 차이가 있기 때문이겠죠. 여기서는 Generation과 Verification의 차이가 모델 학습량의 증가에 따라 증가한다는 것, 그리고 이 갭과 Diversity가 Self Improvement 과정에서 빠르게 감소한다는 것을 발견했습니다.

<english>
Self improvement is possible because of there are difference between generation and verification. In this paper the author observed the gap between generation and verification widens along with increase of model training, and this gap and diversity reduces fast in the process of self improvement.
</english>

#self-improvement #search 