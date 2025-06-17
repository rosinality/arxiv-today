https://arxiv.org/abs/2504.01017

*Scaling Language-Free Visual Representation Learning* (David Fan, Shengbang Tong, Jiachen Zhu, Koustuv Sinha, Zhuang Liu, Xinlei Chen, Michael Rabbat, Nicolas Ballas, Yann LeCun, Amir Bar, Saining Xie)

> Visual Self-Supervised Learning (SSL) currently underperforms Contrastive Language-Image Pretraining (CLIP) in multimodal settings such as Visual Question Answering (VQA). This multimodal gap is often attributed to the semantics introduced by language supervision, even though visual SSL and CLIP models are often trained on different data. In this work, we ask the question: "Do visual self-supervised approaches lag behind CLIP due to the lack of language supervision, or differences in the training data?" We study this question by training both visual SSL and CLIP models on the same MetaCLIP data, and leveraging VQA as a diverse testbed for vision encoders. In this controlled setup, visual SSL models scale better than CLIP models in terms of data and model capacity, and visual SSL performance does not saturate even after scaling up to 7B parameters. Consequently, we observe visual SSL methods achieve CLIP-level performance on a wide range of VQA and classic vision benchmarks. These findings demonstrate that pure visual SSL can match language-supervised visual pretraining at scale, opening new opportunities for vision-centric representation learning.

이미지 SSL 방법이 CLIP에 대비해서 경쟁력 있거나 우수한 Scaling 특성이 나타난다는 연구.

저는 이미지에서는 텍스트로는 완전히 포착되지 않는 특징들을 추출하는 것이 의미있으리라고 생각합니다. 물론 여기서 다룬 건 VQA이긴 하지만요.

<english>
The research suggests image-only SSL has competitive or even better scaling characteristics compared to CLIP.

I think it is meaning to extract features from the images that cannot be captured solely from texts. This study dealt with mainly on VQA, though.
</english>

#clip #self-supervision #scaling-law 