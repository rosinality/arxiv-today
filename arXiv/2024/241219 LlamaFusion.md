https://arxiv.org/abs/2412.15188

*LlamaFusion: Adapting Pretrained Language Models for Multimodal Generation* (Weijia Shi, Xiaochuang Han, Chunting Zhou, Weixin Liang, Xi Victoria Lin, Luke Zettlemoyer, Lili Yu)

> We present LlamaFusion, a framework for empowering pretrained text-only large language models (LLMs) with multimodal generative capabilities, enabling them to understand and generate both text and images in arbitrary sequences. LlamaFusion leverages existing Llama-3's weights for processing texts autoregressively while introducing additional and parallel transformer modules for processing images with diffusion. During training, the data from each modality is routed to its dedicated modules: modality-specific feedforward layers, query-key-value projections, and normalization layers process each modality independently, while the shared self-attention layers allow interactions across text and image features. By freezing the text-specific modules and only training the image-specific modules, LlamaFusion preserves the language capabilities of text-only LLMs while developing strong visual understanding and generation abilities. Compared to methods that pretrain multimodal generative models from scratch, our experiments demonstrate that, LlamaFusion improves image understanding by 20% and image generation by 3.6% using only 50% of the FLOPs while maintaining Llama-3's language capabilities. We also demonstrate that this framework can adapt existing vision-language models with multimodal generation ability. Overall, this framework not only leverages existing computational investments in text-only LLMs but also enables the parallel development of language and vision capabilities, presenting a promising direction for efficient multimodal model development.

Transfusion을 (https://arxiv.org/abs/2408.11039) Llama 3 체크포인트를 재활용해 학습한 모델. 다만 이미지와 텍스트 모달리티에 대해 서로 다른 Attention/FFN Weight를 사용했네요.

<english>
The model which trained Transfusion with recycled Llama 3 checkpoints. But they used distinct attention/ffn weights for each image and text modalities.
</english>

#image-generation #diffusion

# Links

[[240820 Transfusion.md]]