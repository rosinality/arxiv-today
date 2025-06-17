https://arxiv.org/abs/2406.16852

*Long Context Transfer from Language to Vision* (Peiyuan Zhang, Kaichen Zhang, Bo Li, Guangtao Zeng, Jingkang Yang, Yuanhan Zhang, Ziyue Wang, Haoran Tan, Chunyuan Li, Ziwei Liu)

> Video sequences offer valuable temporal information, but existing large multimodal models (LMMs) fall short in understanding extremely long videos. Many works address this by reducing the number of visual tokens using visual resamplers. Alternatively, in this paper, we approach this problem from the perspective of the language model. By simply extrapolating the context length of the language backbone, we enable LMMs to comprehend orders of magnitude more visual tokens without any video training. We call this phenomenon long context transfer and carefully ablate its properties. To effectively measure LMMs' ability to generalize to long contexts in the vision modality, we develop V-NIAH (Visual Needle-In-A-Haystack), a purely synthetic long vision benchmark inspired by the language model's NIAH test. Our proposed Long Video Assistant (LongVA) can process 2000 frames or over 200K visual tokens without additional complexities. With its extended context length, LongVA achieves state-of-the-art performance on Video-MME among 7B-scale models by densely sampling more input frames. Our work is open-sourced at https://github.com/EvolvingLMMs-Lab/LongVA.

Long Context LLM을 이미지-텍스트 페어에 대해서만 정렬한 다음 테스트 시점에서는 이미지 대신 비디오를 입력해봤습니다. 텍스트에 대한 Long Context 능력이 이미지에 대해서도 일반화 되고 모달리티를 뛰어넘을 수도 있다는 결과네요.

전반적으로 Long Context 능력은 Positional Encoding과 모델이 어떤 Attention 분포를 경험했는가의 문제가 아닌가 하는 생각이 있습니다.

#video-language #long-context 