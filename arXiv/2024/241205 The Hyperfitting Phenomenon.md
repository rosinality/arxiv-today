https://arxiv.org/abs/2412.04318

*The Hyperfitting Phenomenon: Sharpening and Stabilizing LLMs for Open-Ended Text Generation* (Fredrik Carlsson, Fangyu Liu, Daniel Ward, Murathan Kurfali, Joakim Nivre)

> This paper introduces the counter-intuitive generalization results of overfitting pre-trained large language models (LLMs) on very small datasets. In the setting of open-ended text generation, it is well-documented that LLMs tend to generate repetitive and dull sequences, a phenomenon that is especially apparent when generating using greedy decoding. This issue persists even with state-of-the-art LLMs containing billions of parameters, trained via next-token prediction on large datasets. We find that by further fine-tuning these models to achieve a near-zero training loss on a small set of samples -- a process we refer to as hyperfitting -- the long-sequence generative capabilities are greatly enhanced. Greedy decoding with these Hyperfitted models even outperform Top-P sampling over long-sequences, both in terms of diversity and human preferences. This phenomenon extends to LLMs of various sizes, different domains, and even autoregressive image generation. We further find this phenomena to be distinctly different from that of Grokking and double descent. Surprisingly, our experiments indicate that hyperfitted models rarely fall into repeating sequences they were trained on, and even explicitly blocking these sequences results in high-quality output. All hyperfitted models produce extremely low-entropy predictions, often allocating nearly all probability to a single token.

LM을 소규모 샘플에 대해 학습 Loss가 0이 될 때까지 학습시키면 Greedy 샘플링을 했을 때 생성되는 데이터의 품질이 향상된다는 결과. Top-1 토큰에 대한 선택이 향상되는 동시에 엔트로피가 크게 낮아지네요. SFT에서 기대되는 효과와 비슷한 것이 아닐까 싶습니다.

<english>
The result that we can enhance quality of generated text with greedy sampling by training LM on small number of sample until training loss becomes 0. Quality of top-1 token enhances, and simultaneously entropy is greatly decreases. I think it is similar effect that we expect in SFT.
</english>

#autoregressive-model 