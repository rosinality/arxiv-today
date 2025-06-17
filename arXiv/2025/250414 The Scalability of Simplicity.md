https://arxiv.org/abs/2504.10462

*The Scalability of Simplicity: Empirical Analysis of Vision-Language Learning with a Single Transformer* (Weixian Lei, Jiacong Wang, Haochen Wang, Xiangtai Li, Jun Hao Liew, Jiashi Feng, Zilong Huang)

> This paper introduces SAIL, a single transformer unified multimodal large language model (MLLM) that integrates raw pixel encoding and language decoding within a singular architecture. Unlike existing modular MLLMs, which rely on a pre-trained vision transformer (ViT), SAIL eliminates the need for a separate vision encoder, presenting a more minimalist architecture design. Instead of introducing novel architectural components, SAIL adapts mix-attention mechanisms and multimodal positional encodings to better align with the distinct characteristics of visual and textual modalities. We systematically compare SAIL's properties-including scalability, cross-modal information flow patterns, and visual representation capabilities-with those of modular MLLMs. By scaling both training data and model size, SAIL achieves performance comparable to modular MLLMs. Notably, the removal of pretrained ViT components enhances SAIL's scalability and results in significantly different cross-modal information flow patterns. Moreover, SAIL demonstrates strong visual representation capabilities, achieving results on par with ViT-22B in vision tasks such as semantic segmentation. Code and models are available at https://github.com/bytedance/SAIL.

이미지 인코더 없는 멀티모달 모델 디자인이 다시 나오기 시작하는군요. Bidirectional Attention 같은 그 나름대로 성가신 요소들이 추가되긴 했습니다만.

<english>
Multimodal model design without image encoder appears again. Some cumbersome elements like bidrectional attention is added, though.
</english>

#multimodal 