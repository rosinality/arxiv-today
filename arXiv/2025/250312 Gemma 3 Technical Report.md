https://storage.googleapis.com/deepmind-media/gemma/Gemma3Report.pdf

*Gemma 3 Technical Report* (Gemma Team, Google DeepMind)

> We introduce Gemma 3, a multimodal addition to the Gemma family of lightweight open models, ranging in scale from 1 to 27 billion parameters. This version introduces vision understanding abilities, a wider coverage of languages and longer context – at least 128K tokens. We also change the architecture of the model to reduce the KV-cache memory that tends to explode with long context. This is achieved by increasing the ratio of local to global attention layers, and keeping the span on local attention short.
> The Gemma 3 models are trained with distillation and achieve superior performance to Gemma 2 for both pre-trained and instruction finetuned versions. In particular, our novel post-training recipe significantly improves the math, chat, instruction-following and multilingual abilities, making Gemma34B-IT competitive with Gemma2-27B-IT and Gemma3-27B-IT comparable to Gemini-1.5-Pro across benchmarks. We release all our models to the community.

Gemma 3가 나왔네요. Softcapping 대신 QK Norm을 썼군요. Window와 Global Attention의 조합에서 Window Attention의 비율을 5:1로 늘리면서 128K Context Length로 확장. 그리고 이미지 인식 능력을 탑재했습니다. 포스트트레이닝에는 구글이 그동안 공개했던 방법들의 종합에 (https://arxiv.org/abs/2407.14622, https://arxiv.org/abs/2401.12187, https://arxiv.org/abs/2406.16768) Verifiable Reward를 추가했군요.

<english>
Gemma 3 appeared. They used QK norm instead of softcapping. They increased ratio of window attention to 5:1 on combination of window and global attentions, and extended context length to 128K. Also they added image recognition capability. For post-training they used combination of method that Google have been released (https://arxiv.org/abs/2407.14622, https://arxiv.org/abs/2401.12187, https://arxiv.org/abs/2406.16768) and added verifiable rewards.
</english>

#llm #vision-language 