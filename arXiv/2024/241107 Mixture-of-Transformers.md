https://arxiv.org/abs/2411.04996

*Mixture-of-Transformers: A Sparse and Scalable Architecture for Multi-Modal Foundation Models* (Weixin Liang, Lili Yu, Liang Luo, Srinivasan Iyer, Ning Dong, Chunting Zhou, Gargi Ghosh, Mike Lewis, Wen-tau Yih, Luke Zettlemoyer, Xi Victoria Lin)

> The development of large language models (LLMs) has expanded to multi-modal systems capable of processing text, images, and speech within a unified framework. Training these models demands significantly larger datasets and computational resources compared to text-only LLMs. To address the scaling challenges, we introduce Mixture-of-Transformers (MoT), a sparse multi-modal transformer architecture that significantly reduces pretraining computational costs. MoT decouples non-embedding parameters of the model by modality -- including feed-forward networks, attention matrices, and layer normalization -- enabling modality-specific processing with global self-attention over the full input sequence. We evaluate MoT across multiple settings and model scales. In the Chameleon 7B setting (autoregressive text-and-image generation), MoT matches the dense baseline's performance using only 55.8\% of the FLOPs. When extended to include speech, MoT reaches speech performance comparable to the dense baseline with only 37.2\% of the FLOPs. In the Transfusion setting, where text and image are trained with different objectives, a 7B MoT model matches the image modality performance of the dense baseline with one third of the FLOPs, and a 760M MoT model outperforms a 1.4B dense baseline across key image generation metrics. System profiling further highlights MoT's practical benefits, achieving dense baseline image quality in 47.2\% of the wall-clock time and text quality in 75.6\% of the wall-clock time (measured on AWS p4de.24xlarge instances with NVIDIA A100 GPUs).

동일한 트랜스포머 레이어로 모든 모달리티를 커버하게 하는 경우에도 각 모달리티에 따라 임베딩이 독립적으로 움직이니, 각 모달리티에 따라 서로 다른 트랜스포머 레이어를 적용하고 모달리티 사이의 Global Attention을 추가한 구조. 좀 더 극단적으로 나아간 Modality Expert 구조라고 생각할 수 있겠네요.

<english>
As when same transformer layers are applied all of modalities embeddings shows independent behavior among modalities, so instead applies different transformer layers for each modalities, and adds global attention between modalities. It would be more extreme version of modality experts architecture.
</english>

#moe #multimodal #transformer 