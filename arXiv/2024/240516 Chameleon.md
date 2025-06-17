https://arxiv.org/abs/2405.09818

*Chameleon: Mixed-Modal Early-Fusion Foundation Models* (Chameleon Team)

> We present Chameleon, a family of early-fusion token-based mixed-modal models capable of understanding and generating images and text in any arbitrary sequence. We outline a stable training approach from inception, an alignment recipe, and an architectural parameterization tailored for the early-fusion, token-based, mixed-modal setting. The models are evaluated on a comprehensive range of tasks, including visual question answering, image captioning, text generation, image generation, and long-form mixed modal generation. Chameleon demonstrates broad and general capabilities, including state-of-the-art performance in image captioning tasks, outperforms Llama-2 in text-only tasks while being competitive with models such as Mixtral 8x7B and Gemini-Pro, and performs non-trivial image generation, all in a single model. It also matches or exceeds the performance of much larger models, including Gemini Pro and GPT-4V, according to human judgments on a new long-form mixed-modal generation evaluation, where either the prompt or outputs contain mixed sequences of both images and text. Chameleon marks a significant step forward in a unified modeling of full multimodal documents.

드디어 나왔군요. 메타의 Early Fusion Vision Language 모델. VQ-VAE를 사용해 토크나이즈했고 9.2T 학습했네요.

학습 안정성을 위한 세팅들이 흥미롭습니다. QK Norm과 Swin Transformer V2 스타일의 Post Normalization (https://arxiv.org/abs/2111.09883) 혹은 Dropout을 사용했군요.

다만 벤치마크, 특히 이미지 생성에 대한 벤치마크가 적은 걸 보면 좀 급하게 낸 것이 아닌가 싶습니다. 모델 자체는 5개월 전에 학습이 끝났다고 합니다만. (https://x.com/ArmenAgha/status/1791275538625241320)

#vision-language #autoregressive-model

# Links

[[211118 Swin Transformer V2.md]]