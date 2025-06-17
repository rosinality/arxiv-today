https://arxiv.org/abs/2403.17007

*DreamLIP: Language-Image Pre-training with Long Captions* (Kecheng Zheng, Yifei Zhang, Wei Wu, Fan Lu, Shuailei Ma, Xin Jin, Wei Chen, Yujun Shen)

> Language-image pre-training largely relies on how precisely and thoroughly a text describes its paired image. In practice, however, the contents of an image can be so rich that well describing them requires lengthy captions (e.g., with 10 sentences), which are usually missing in existing datasets. Consequently, there are currently no clear evidences on whether and how language-image pre-training could benefit from long captions. To figure this out, we first re-caption 30M images with detailed descriptions using a pre-trained Multi-modality Large Language Model (MLLM), and then study the usage of the resulting captions under a contrastive learning framework. We observe that, each sentence within a long caption is very likely to describe the image partially (e.g., an object). Motivated by this, we propose to dynamically sample sub-captions from the text label to construct multiple positive pairs, and introduce a grouping loss to match the embeddings of each sub-caption with its corresponding local image patches in a self-supervised manner. Experimental results on a wide rage of downstream tasks demonstrate the consistent superiority of our method, termed DreamLIP, over previous alternatives, highlighting its fine-grained representational capacity. It is noteworthy that, on the tasks of image-text retrieval and semantic segmentation, our model trained with 30M image-text pairs achieves on par or even better performance than CLIP trained with 400M pairs. Project page is available at https://zyf0619sjtu.github.io/dream-lip.

긴 캡션을 생성한 다음 이 캡션을 쪼개 부분 캡션들을 만들고 이 캡션들과의 Contrastive Loss + 캡션과 이미지 패치의 Cross Attention 가중치를 Sparse 하게 만든 다음 Contrastive Loss를 적용. (https://arxiv.org/abs/2401.09865) 텍스트 토큰 레벨인가 부분 캡션 레벨인가라는 선택이 하나 발생하는군요.

아예 이미지를 쪼갠 다음 각 부분에 대해 상세한 캡션을 만드는 것을 목표로 했던 사례 (https://arxiv.org/abs/2312.08578) 와 결합해서 생각해보면 좀 더 재미있을 듯 싶습니다.

#clip #synthetic-data

# Links

[[240118 Improving fine-grained understanding in image-text pre-training.md]]
[[231214 A Picture is Worth More Than 77 Text Tokens.md]]