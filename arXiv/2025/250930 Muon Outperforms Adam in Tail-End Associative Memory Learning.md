https://arxiv.org/abs/2509.26030

*Muon Outperforms Adam in Tail-End Associative Memory Learning* (Shuche Wang, Fengzhuo Zhang, Jiaxiang Li, Cunxiao Du, Chao Du, Tianyu Pang, Zhuoran Yang, Mingyi Hong, Vincent Y. F. Tan)

> The Muon optimizer is consistently faster than Adam in training Large Language Models (LLMs), yet the mechanism underlying its success remains unclear. This paper demystifies this mechanism through the lens of associative memory. By ablating the transformer components optimized by Muon, we reveal that the associative memory parameters of LLMs, namely the Value and Output (VO) attention weights and Feed-Forward Networks (FFNs), are the primary contributors to Muon's superiority. Motivated by this associative memory view, we then explain Muon's superiority on real-world corpora, which are intrinsically heavy-tailed: a few classes (tail classes) appear far less frequently than others. The superiority is explained through two key properties: (i) its update rule consistently yields a more isotropic singular spectrum than Adam; and as a result, (ii) on heavy-tailed data, it optimizes tail classes more effectively than Adam. Beyond empirical evidence, we theoretically confirm these findings by analyzing a one-layer associative memory model under class-imbalanced data. We prove that Muon consistently achieves balanced learning across classes regardless of feature embeddings, whereas Adam can induce large disparities in learning errors depending on embedding properties. In summary, our empirical observations and theoretical analyses reveal Muon's core advantage: its update rule aligns with the outer-product structure of linear associative memories, enabling more balanced and effective learning of tail classes in heavy-tailed distributions than Adam.

Muon vs Adam. Muon의 효과는 주로 Attention Value, Output, FFN 행렬에 대한 효과에서 온다고. 그리고 분포의 꼬리 부분의 지식을 더 빠르게 학습. Optimizer Inductive Bias? (https://arxiv.org/abs/2507.12224) 물론 속도의 문제일 수도 있음.

<english>
Muon vs Adam. Gain of Muon mainly comes from the its effect on the attention value and output, FFN matrices. And it learns the knowledges in the tail of the distribution faster. Optimizer inductive biases? (https://arxiv.org/abs/2507.12224) Though it could be matter of the speed.
</english>

#optimization #transformer 