https://arxiv.org/abs/2402.04347

*The Hedgehog & the Porcupine: Expressive Linear Attentions with Softmax Mimicry* (Michael Zhang, Kush Bhatia, Hermann Kumbong, Christopher Ré)

> Linear attentions have shown potential for improving Transformer efficiency, reducing attention's quadratic complexity to linear in sequence length. This holds exciting promise for (1) training linear Transformers from scratch, (2) "finetuned-conversion" of task-specific Transformers into linear versions that recover task performance, and (3) "pretrained-conversion" of Transformers such as large language models into linear versions finetunable on downstream tasks. However, linear attentions often underperform standard softmax attention in quality. To close this performance gap, we find prior linear attentions lack key properties of softmax attention tied to good performance: low-entropy (or "spiky") weights and dot-product monotonicity. We further observe surprisingly simple feature maps that retain these properties and match softmax performance, but are inefficient to compute in linear attention. We thus propose Hedgehog, a learnable linear attention that retains the spiky and monotonic properties of softmax attention while maintaining linear complexity. Hedgehog uses simple trainable MLPs to produce attention weights mimicking softmax attention. Experiments show Hedgehog recovers over 99% of standard Transformer quality in train-from-scratch and finetuned-conversion settings, outperforming prior linear attentions up to 6 perplexity points on WikiText-103 with causal GPTs, and up to 8.7 GLUE score points on finetuned bidirectional BERTs. Hedgehog also enables pretrained-conversion. Converting a pretrained GPT-2 into a linear attention variant achieves state-of-the-art 16.7 perplexity on WikiText-103 for 125M subquadratic decoder models. We finally turn a pretrained Llama-2 7B into a viable linear attention Llama. With low-rank adaptation, Hedgehog-Llama2 7B achieves 28.1 higher ROUGE-1 points over the base standard attention model, where prior linear attentions lead to 16.5 point drops.

Softmax Attention과 Linear Attention 사이의 가장 큰 차이가 Softmax는 엔트로피가 낮은, 즉 특정 위치에 Attention Weight가 집중되는 "뾰족한" 패턴을 보여준다는 것에 있다는 주장. 이를 Tayler 근사로 커버해서 Linear Attention의 성능을 높일 수 있다고 합니다. 이에 더해 Softmax Attention을 Linear Attention으로 Distill하는 것을 시도했네요.

Associative Recall과 관련된 블로그에서 먼저 소개된 결과인데 (https://arxiv.org/abs/2305.01625) 논문으로 나왔군요.

#linear-attention

# Links

[[230502 Unlimiformer.md]]