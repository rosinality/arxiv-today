https://arxiv.org/abs/2410.02740

*Revisit Large-Scale Image-Caption Data in Pre-training Multimodal Foundation Models* (Zhengfeng Lai, Vasileios Saveris, Chen Chen, Hong-You Chen, Haotian Zhang, Bowen Zhang, Juan Lao Tebar, Wenze Hu, Zhe Gan, Peter Grasch, Meng Cao, Yinfei Yang)

> Recent advancements in multimodal models highlight the value of rewritten captions for improving performance, yet key challenges remain. For example, while synthetic captions often provide superior quality and image-text alignment, it is not clear whether they can fully replace AltTexts: the role of synthetic captions and their interaction with original web-crawled AltTexts in pre-training is still not well understood. Moreover, different multimodal foundation models may have unique preferences for specific caption formats, but efforts to identify the optimal captions for each model remain limited. In this work, we propose a novel, controllable, and scalable captioning pipeline designed to generate diverse caption formats tailored to various multimodal models. By examining Short Synthetic Captions (SSC) towards Dense Synthetic Captions (DSC+) as case studies, we systematically explore their effects and interactions with AltTexts across models such as CLIP, multimodal LLMs, and diffusion models. Our findings reveal that a hybrid approach that keeps both synthetic captions and AltTexts can outperform the use of synthetic captions alone, improving both alignment and performance, with each model demonstrating preferences for particular caption formats. This comprehensive analysis provides valuable insights into optimizing captioning strategies, thereby advancing the pre-training of multimodal foundation models.

이미지-텍스트 페어에서 합성 데이터의 사용, 특히 여러 합성 데이터의 스타일(상세한 정도, Alt Text를 결합하는 여부 등), 그리고 CLIP/Multimodal LLM/Text-to-Image 모델에 대한 비교 분석. 상세한 캡션이 좋고 Alt Text를 결합하는 것이 종종 좋을 수 있다는 느낌이네요. 

<english>
Comparative analysis on using synthetic data for image-text pairs, especially various styles of synthetic captions (detailedness, whether fuse alt text), and CLIP/Multimodal LLM/Text-to-Image models. Long story short detailed captions is best, and often using alt text is beneficial.
</english>

#synthetic-data #image-text #captioning 