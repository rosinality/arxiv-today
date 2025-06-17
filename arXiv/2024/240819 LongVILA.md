https://arxiv.org/abs/2408.10188

*LongVILA: Scaling Long-Context Visual Language Models for Long Videos* (Fuzhao Xue, Yukang Chen, Dacheng Li, Qinghao Hu, Ligeng Zhu, Xiuyu Li, Yunhao Fang, Haotian Tang, Shang Yang, Zhijian Liu, Ethan He, Hongxu Yin, Pavlo Molchanov, Jan Kautz, Linxi Fan, Yuke Zhu, Yao Lu, Song Han)

> Long-context capability is critical for multi-modal foundation models. We introduce LongVILA, a full-stack solution for long-context vision-language models, including system, model training, and dataset development. On the system side, we introduce the first Multi-Modal Sequence Parallelism (MM-SP) system that enables long-context training and inference, enabling 2M context length training on 256 GPUs. MM-SP is also efficient, being 2.1x - 5.7x faster than Ring-Style Sequence Parallelism and 1.1x - 1.4x faster than Megatron-LM in text-only settings. Moreover, it seamlessly integrates with Hugging Face Transformers. For model training, we propose a five-stage pipeline comprising alignment, pre-training, context extension, and long-short joint supervised fine-tuning. Regarding datasets, we meticulously construct large-scale visual language pre-training datasets and long video instruction-following datasets to support our multi-stage training process. The full-stack solution extends the feasible frame number of VILA by a factor of 128 (from 8 to 1024 frames) and improves long video captioning score from 2.00 to 3.26 (1.6x), achieving 99.5% accuracy in 1400-frames video (274k context length) needle in a haystack. LongVILA-8B also demonstrates a consistent improvement in performance on long videos within the VideoMME benchmark as the video frames increase.

Long Context 모델로 길이가 긴 비디오를 태클. Long Context 모델로 이미지에서 비디오로 Transfer한 시도가 떠오르네요. (https://arxiv.org/abs/2406.16852) 여기서도 이미지/짧은 비디오로 Multimodal Alignment를 한 다음 Long Context로 확장하고 다시 긴 길이의 비디오로 튜닝하는 방법을 따랐습니다.

재미있는 부분은 Multimodal Long Context 모델을 학습하기 위한 인프라네요. 노드 내에서는 DeepSpeed-Ulysses 스타일의 헤드를 나누는 Sequence Parallel을 사용하고 노드 간에는 시퀀스를 나누는 Ring Attention을 사용했습니다.

#video-text #long-context

# Links

[[240624 Long Context Transfer from Language to Vision.md]]