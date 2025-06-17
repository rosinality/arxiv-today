https://arxiv.org/abs/2401.06129

*Distilling Vision-Language Models on Millions of Videos* (Yue Zhao, Long Zhao, Xingyi Zhou, Jialin Wu, Chun-Te Chu, Hui Miao, Florian Schroff, Hartwig Adam, Ting Liu, Boqing Gong, Philipp Krähenbühl, Liangzhe Yuan)

> The recent advance in vision-language models is largely attributed to the abundance of image-text data. We aim to replicate this success for video-language models, but there simply is not enough human-curated video-text data available. We thus resort to fine-tuning a video-language model from a strong image-language baseline with synthesized instructional data. The resulting video-language model is then used to auto-label millions of videos to generate high-quality captions. We show the adapted video-language model performs well on a wide range of video-language benchmarks. For instance, it surpasses the best prior result on open-ended NExT-QA by 2.8%. Besides, our model generates detailed descriptions for previously unseen videos, which provide better textual supervision than existing methods. Experiments show that a video-language dual-encoder model contrastively trained on these auto-generated captions is 3.8% better than the strongest baseline that also leverages vision-language models. Our best model outperforms state-of-the-art methods on MSR-VTT zero-shot text-to-video retrieval by 6%.

이미지에 대한 캡션 새로 달기가 비디오로 넘어왔군요. VLM에서 시작해 LM은 얼리고 Vision Encoder를 학습시킵니다. 저품질의 캡션에 LM이 영향을 받는 것을 막기 위함이죠. 이후 좀 더 고품질의 Instruction 데이터로 LM을 튜닝합니다.이렇게 만든 모델로 캡션을 새로 달아서 Constrastive Learning 등에 쓸 수 있었다고 합니다.

#video-language #multimodal 