https://arxiv.org/abs/2410.16166

*Beyond Filtering: Adaptive Image-Text Quality Enhancement for MLLM Pretraining* (Han Huang, Yuqi Huo, Zijia Zhao, Haoyu Lu, Shu Wu, Bingning Wang, Qiang Liu, Weipeng Chen, Liang Wang)

> Multimodal large language models (MLLMs) have made significant strides by integrating visual and textual modalities. A critical factor in training MLLMs is the quality of image-text pairs within multimodal pretraining datasets. However, $\textit {de facto}$ filter-based data quality enhancement paradigms often discard a substantial portion of high-quality image data due to inadequate semantic alignment between images and texts, leading to inefficiencies in data utilization and scalability. In this paper, we propose the Adaptive Image-Text Quality Enhancer (AITQE), a model that dynamically assesses and enhances the quality of image-text pairs. AITQE employs a text rewriting mechanism for low-quality pairs and incorporates a negative sample learning strategy to improve evaluative capabilities by integrating deliberately selected low-quality samples during training. Unlike prior approaches that significantly alter text distributions, our method minimally adjusts text to preserve data volume while enhancing quality. Experimental results demonstrate that AITQE surpasses existing methods on various benchmark, effectively leveraging raw data and scaling efficiently with increasing data volumes. We hope our work will inspire future works. The code and model are available at: https://github.com/hanhuang22/AITQE.

이미지-텍스트 데이터의 품질 평가와 캡션 재작성을 수행하는 모델 개발. 품질이 높은 데이터는 그대로 사용하고 품질이 낮은 경우 캡션을 재작성한다는 아이디어네요. 캡션 재작성은 이제 기본적인 도구가 되었는데 이를 잘 하는 것이 중요한 예술이 되었다는 느낌이네요.

<english>
Developing the model doing quality assessment of image-text data and recaptioning. We can use high quality data as-is, and recaption low quality data. Recaptioning is now became basic tool, and I think it is important technique how to do well in recaptioning now.
</english>

#multimodal #captioning #dataset 