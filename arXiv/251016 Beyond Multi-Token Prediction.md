https://arxiv.org/abs/2510.14751

*Beyond Multi-Token Prediction: Pretraining LLMs with Future Summaries* (Divyat Mahajan, Sachin Goyal, Badr Youbi Idrissi, Mohammad Pezeshki, Ioannis Mitliagkas, David Lopez-Paz, Kartik Ahuja)

> Next-token prediction (NTP) has driven the success of large language models (LLMs), but it struggles with long-horizon reasoning, planning, and creative writing, with these limitations largely attributed to teacher-forced training. Multi-token prediction (MTP) partially mitigates these issues by predicting several future tokens at once, but it mostly captures short-range dependencies and offers limited improvement. We propose future summary prediction (FSP), which trains an auxiliary head to predict a compact representation of the long-term future, preserving information relevant for long-form generations. We explore two variants of FSP: handcrafted summaries, for example, a bag of words summary of the future of the sequence, and learned summaries, which use embeddings produced by a reverse language model trained from right to left. Large-scale pretraining experiments (3B and 8B-parameter models) demonstrate that FSP provides improvements over both NTP and MTP across math, reasoning, and coding benchmarks.

Bag of Tokens나 Reverse LM의 Feature를 예측하게 하는 것으로 MTP 개선. Speculative Decoding을 고려했을 때 Block Diffusion과 같은 구조를 MTP와 연결하는 것은 괜찮은 방법일지도?

<english>
Improving MTP by let model to predict future bag of tokens or a feature from reverse LM. Considering speculative decoding, something like block diffusion could be a nice way to deal with this?
</english>

#pretraining 