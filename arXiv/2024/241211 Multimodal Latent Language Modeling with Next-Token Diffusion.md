https://arxiv.org/abs/2412.08635

*Multimodal Latent Language Modeling with Next-Token Diffusion* (Yutao Sun, Hangbo Bao, Wenhui Wang, Zhiliang Peng, Li Dong, Shaohan Huang, Jianyong Wang, Furu Wei)

> Multimodal generative models require a unified approach to handle both discrete data (e.g., text and code) and continuous data (e.g., image, audio, video). In this work, we propose Latent Language Modeling (LatentLM), which seamlessly integrates continuous and discrete data using causal Transformers. Specifically, we employ a variational autoencoder (VAE) to represent continuous data as latent vectors and introduce next-token diffusion for autoregressive generation of these vectors. Additionally, we develop $\sigma$-VAE to address the challenges of variance collapse, which is crucial for autoregressive modeling. Extensive experiments demonstrate the effectiveness of LatentLM across various modalities. In image generation, LatentLM surpasses Diffusion Transformers in both performance and scalability. When integrated into multimodal large language models, LatentLM provides a general-purpose interface that unifies multimodal generation and understanding. Experimental results show that LatentLM achieves favorable performance compared to Transfusion and vector quantized models in the setting of scaling up training tokens. In text-to-speech synthesis, LatentLM outperforms the state-of-the-art VALL-E 2 model in speaker similarity and robustness, while requiring 10x fewer decoding steps. The results establish LatentLM as a highly effective and scalable approach to advance large multimodal models.

VAE로 Continuous Token으로 변환한 다음 Diffusion Head로 Autoregressive Generation. Transfusion (https://arxiv.org/abs/2408.11039) 같은 계통의 아이디어인데 (https://arxiv.org/abs/2406.11838) 가장 단순한 형태의 Next Token Prediction을 사용했다고 할 수 있겠네요.

추론 속도의 특성 등이 좀 더 궁금하긴 한데 여튼 이쪽도 좋은 방향입니다.

<english>
Autoregress generation by predicting continuous tokens transformed using VAE with diffusion head. The idea is in vein of Transfusion (https://arxiv.org/abs/2408.11039) and similar approaches (https://arxiv.org/abs/2406.11838) but this study used simplest approach of next token prediction.

I wonder about charateristics of inference performances, but anyway, this is promising approach.
</english>

#autoregressive-model #vae #diffusion

# Links

[[240820 Transfusion.md]]
[[240617 Autoregressive Image Generation without Vector Quantization.md]]