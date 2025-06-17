https://arxiv.org/abs/2405.09719

*Spectral Editing of Activations for Large Language Model Alignment* (Yifu Qiu, Zheng Zhao, Yftah Ziser, Anna Korhonen, Edoardo M. Ponti, Shay B. Cohen)

> Large language models (LLMs) often exhibit undesirable behaviours, such as generating untruthful or biased content. Editing their internal representations has been shown to be effective in mitigating such behaviours on top of the existing alignment methods. We propose a novel inference-time editing method, namely spectral editing of activations (SEA), to project the input representations into directions with maximal covariance with the positive demonstrations (e.g., truthful) while minimising covariance with the negative demonstrations (e.g., hallucinated). We also extend our method to non-linear editing using feature functions. We run extensive experiments on benchmarks concerning truthfulness and bias with six open-source LLMs of different sizes and model families. The results demonstrate the superiority of SEA in effectiveness, generalisation to similar tasks, as well as inference and data efficiency. We also show that SEA editing only has a limited negative impact on other model capabilities.

Activation Editing을 통한 정렬. Positive와 Negative 예시에 대한 임베딩을 얻고 Positive 임베딩에 대한 공분산을 최대화/Negative에 대한 공분산을 최소화 하는 형태군요. 적당한 수의 데이터로 튜닝 데이터 구축을 위한 부트스트래핑에 쓸 수 있을까 싶습니다.

#alignment 