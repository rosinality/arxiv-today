https://arxiv.org/abs/2401.06751

*The Unreasonable Effectiveness of Easy Training Data for Hard Tasks* (Peter Hase, Mohit Bansal, Peter Clark, Sarah Wiegreffe)

> How can we train models to perform well on hard test data when hard training data is by definition difficult to label correctly? This question has been termed the scalable oversight problem and has drawn increasing attention as language models have continually improved. In this paper, we present the surprising conclusion that current language models often generalize relatively well from easy to hard data, even performing as well as "oracle" models trained on hard data. We demonstrate this kind of easy-to-hard generalization using simple training methods like in-context learning, linear classifier heads, and QLoRA for seven different measures of datapoint hardness, including six empirically diverse human hardness measures (like grade level) and one model-based measure (loss-based). Furthermore, we show that even if one cares most about model performance on hard data, it can be better to collect and train on easy data rather than hard data, since hard data is generally noisier and costlier to collect. Our experiments use open models up to 70b in size and four publicly available question-answering datasets with questions ranging in difficulty from 3rd grade science questions to college level STEM questions and general-knowledge trivia. We conclude that easy-to-hard generalization in LMs is surprisingly strong for the tasks studied, suggesting the scalable oversight problem may be easier than previously thought. Our code is available at https://github.com/allenai/easy-to-hard-generalization

쉬운 문제로 학습시켰을 때 어려운 문제에 대한 성능을 높일 수 있는가? 사실 난이도를 정의하는 것부터 쉽지 않죠. 사람 기준으로 평가하는 난이도와 모델 기준의 난이도가 같으리라는 보장은 없고 실제로 꽤 다른 것으로 보입니다.

모델에 대해서 알고자 한다면 모델 기준의 난이도가 의미가 있겠지만, 사람 기준의 난이도도 데이터 구축 비용을 줄여줄 수 있으니 의미가 있겠죠.

여하간 이러한 난이도 지표를 통해 살펴봤을 때 쉬운 데이터로 튜닝했을 때에도 어려운 데이터로 튜닝한 것의 성능을 70% 이상 복원할 수 있는 경우가 많았다는 이야기를 하고 있습니다. 튜닝 방법이나 난이도의 간격 등 변수들이 많긴 하지만 쉬운 문제로 어려운 문제를 풀 수 있다는 것의 함의는 굉장하겠죠. (그리고 어려운 문제로 더 어려운 문제를 풀 수 있는가가 흥미로운 부분이 되겠죠.)

#dataset #in_context_learning 
