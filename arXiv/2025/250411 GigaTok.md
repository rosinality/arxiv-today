https://arxiv.org/abs/2504.08736

*GigaTok: Scaling Visual Tokenizers to 3 Billion Parameters for Autoregressive Image Generation* (Tianwei Xiong, Jun Hao Liew, Zilong Huang, Jiashi Feng, Xihui Liu)

> In autoregressive (AR) image generation, visual tokenizers compress images into compact discrete latent tokens, enabling efficient training of downstream autoregressive models for visual generation via next-token prediction. While scaling visual tokenizers improves image reconstruction quality, it often degrades downstream generation quality -- a challenge not adequately addressed in existing literature. To address this, we introduce GigaTok, the first approach to simultaneously improve image reconstruction, generation, and representation learning when scaling visual tokenizers. We identify the growing complexity of latent space as the key factor behind the reconstruction vs. generation dilemma. To mitigate this, we propose semantic regularization, which aligns tokenizer features with semantically consistent features from a pre-trained visual encoder. This constraint prevents excessive latent space complexity during scaling, yielding consistent improvements in both reconstruction and downstream autoregressive generation. Building on semantic regularization, we explore three key practices for scaling tokenizers:(1) using 1D tokenizers for better scalability, (2) prioritizing decoder scaling when expanding both encoder and decoder, and (3) employing entropy loss to stabilize training for billion-scale tokenizers. By scaling to $\bf{3 \space billion}$ parameters, GigaTok achieves state-of-the-art performance in reconstruction, downstream AR generation, and downstream AR representation quality.

VQ 토크나이저 Scaling. DINOv2를 사용한 Semantic Regularization이 필수적이군요.

<english>
Scaling VQ tokenizers. It is crucial to apply semantic regularization using DINOv2.
</english>

#vq #tokenizer 