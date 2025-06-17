https://arxiv.org/abs/2506.06215

*Corrector Sampling in Language Models* (Itai Gat, Neta Shaul, Uriel Singer, Yaron Lipman)

> Autoregressive language models accumulate errors due to their fixed, irrevocable left-to-right token generation. To address this, we propose a new sampling method called Resample-Previous-Tokens (RPT). RPT mitigates error accumulation by iteratively revisiting and potentially replacing tokens in a window of previously generated text. This method can be integrated into existing autoregressive models, preserving their next-token-prediction quality and speed. Fine-tuning a pretrained 8B parameter model with RPT for only 100B resulted in ~10% relative improvements on reasoning and coding benchmarks compared to the standard sampling.

이전에 샘플링한 토큰의 에러를 교정하는 학습 Objective. 시퀀스 내의 일정 토큰들의 위치를 옮긴 다음 그 위치에 있었어야할 토큰을 예측하게 하는군요.

<english>
Training objective that corrects error on previously sampled tokens. It moves the position of token segment in the sequence and let model to predict the token that original exists at that.
</english>

#llm #decoding 