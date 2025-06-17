https://arxiv.org/abs/2408.16357

*Law of Vision Representation in MLLMs* (Shijia Yang, Bohan Zhai, Quanzeng You, Jianbo Yuan, Hongxia Yang, Chenfeng Xu)

> We present the "Law of Vision Representation" in multimodal large language models (MLLMs). It reveals a strong correlation between the combination of cross-modal alignment, correspondence in vision representation, and MLLM performance. We quantify the two factors using the cross-modal Alignment and Correspondence score (AC score). Through extensive experiments involving thirteen different vision representation settings and evaluations across eight benchmarks, we find that the AC score is linearly correlated to model performance. By leveraging this relationship, we are able to identify and train the optimal vision representation only, which does not require finetuning the language model every time, resulting in a 99.7% reduction in computational cost.

Vision Language 모델의 성능은 이미지 인코더의 출력 Feature가 언어와 얼마나 잘 정렬되어 있는가, 그리고 이미지에 대한 Correspondence를 추출하기 용이한 형태인가로 계산 가능하다는 주장. 물론 이 둘을 어떻게 측정할 것인가가 문제이긴 합니다.

언어와 잘 정렬되어 있으면서 Semantic한 디테일까지 잘 포착한다면 충분히 좋은 이미지 인코더가 되긴 하겠죠.

 #vision-language 