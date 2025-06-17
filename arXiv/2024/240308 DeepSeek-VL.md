https://arxiv.org/abs/2403.05525

*DeepSeek-VL: Towards Real-World Vision-Language Understanding* (Haoyu Lu, Wen Liu, Bo Zhang, Bingxuan Wang, Kai Dong, Bo Liu, Jingxiang Sun, Tongzheng Ren, Zhuoshu Li, Yaofeng Sun, Chengqi Deng, Hanwei Xu, Zhenda Xie, Chong Ruan)

> We present DeepSeek-VL, an open-source Vision-Language (VL) Model designed for real-world vision and language understanding applications. Our approach is structured around three key dimensions: We strive to ensure our data is diverse, scalable, and extensively covers real-world scenarios including web screenshots, PDFs, OCR, charts, and knowledge-based content, aiming for a comprehensive representation of practical contexts. Further, we create a use case taxonomy from real user scenarios and construct an instruction tuning dataset accordingly. The fine-tuning with this dataset substantially improves the model's user experience in practical applications. Considering efficiency and the demands of most real-world scenarios, DeepSeek-VL incorporates a hybrid vision encoder that efficiently processes high-resolution images (1024 x 1024), while maintaining a relatively low computational overhead. This design choice ensures the model's ability to capture critical semantic and detailed information across various visual tasks. We posit that a proficient Vision-Language Model should, foremost, possess strong language abilities. To ensure the preservation of LLM capabilities during pretraining, we investigate an effective VL pretraining strategy by integrating LLM training from the beginning and carefully managing the competitive dynamics observed between vision and language modalities. The DeepSeek-VL family (both 1.3B and 7B models) showcases superior user experiences as a vision-language chatbot in real-world applications, achieving state-of-the-art or competitive performance across a wide range of visual-language benchmarks at the same model size while maintaining robust performance on language-centric benchmarks. We have made both 1.3B and 7B models publicly accessible to foster innovations based on this foundation model.

DeepSeek의 Vision Language 모델이군요. 흥미로운 부분들.

1. 이미지2코드와 OCR 데이터셋의 구축 및 추가
2. Low Resolution SigLIP와 High Resolution SAM 인코더
3. 어댑터 학습 - 전체 학습 - SFT라는 일반적인 단계
4. 1.3B 모델로 7B로 Scaling 과정의 난점. 1.3B는 모델의 성능 문제로 학습 과정 중 메트릭의 요동이 심함. SFT 데이터를 약간 넣고 Perplexity 기반으로 답을 고르는 것으로 수정
5. 텍스트 임베딩과 Vision Encoder를 묶어서 하나의 Pipeline Block으로 취급

CLIP에 추가 인코더를 사용해서 본격적으로 결과를 본 사례가 드디어 등장했군요.

여담이지만 Anna's Archive의 책 데이터를 사용했다고 명시하고 있습니다. 이 책 데이터가 암암리에 쓰이고 있다는 이야기가 있는데 그걸 확인해줬네요.

#vision-language 