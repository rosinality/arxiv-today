https://arxiv.org/abs/2504.07951

*Scaling Laws for Native Multimodal Models* (Mustafa Shukor, Enrico Fini, Victor Guilherme Turrisi da Costa, Matthieu Cord, Joshua Susskind, Alaaeldin El-Nouby)

> Building general-purpose models that can effectively perceive the world through multimodal signals has been a long-standing goal. Current approaches involve integrating separately pre-trained components, such as connecting vision encoders to LLMs and continuing multimodal training. While such approaches exhibit remarkable sample efficiency, it remains an open question whether such late-fusion architectures are inherently superior. In this work, we revisit the architectural design of native multimodal models (NMMs)--those trained from the ground up on all modalities--and conduct an extensive scaling laws study, spanning 457 trained models with different architectures and training mixtures. Our investigation reveals no inherent advantage to late-fusion architectures over early-fusion ones, which do not rely on image encoders. On the contrary, early-fusion exhibits stronger performance at lower parameter counts, is more efficient to train, and is easier to deploy. Motivated by the strong performance of the early-fusion architectures, we show that incorporating Mixture of Experts (MoEs) allows for models that learn modality-specific weights, significantly enhancing performance.

From Scratch 학습한 Multimodal 모델에 대한 Scaling Law. ViT 없는 Early Fusion과 Late Fusion에서는 큰 차이가 나지 않고, (최적 Paramter vs Data 할당 비율은 다릅니다.) 모달리티를 구분하지 않는 MoE가 구분하는 쪽보다 낫군요.

<english>
A scaling law for from scratch trained multimodal models. There are no large difference between early fusion without ViT and late fusion (It has different ratio of optimal parameter and data allocation, though) and modality agnostic MoE is better than modality aware routing.
</english>

#scaling-law #multimodal 