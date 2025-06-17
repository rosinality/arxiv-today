https://arxiv.org/abs/2312.08578

A Picture is Worth More Than 77 Text Tokens: Evaluating CLIP-Style Models on Dense Captions (Jack Urbanek, Florian Bordes, Pietro Astolfi, Mary Williamson, Vasu Sharma, Adriana Romero-Soriano)

요즘 관심이 뜨거운 웹 이미지-텍스트 페어의 캡션 퀄리티 문제에 대한 접근. 전체 이미지와 SAM으로 뽑은 마스크를 사용해 평균 1,111 단어 분량의 굉장히 상세한 캡션이 달린 데이터셋을 만들었습니다.

이걸로 CLIP을 평가하려고 하니 단어가 너무 많아서 쓸 수가 없어 요약 버전을 만들었군요. 이 요약 버전으로 VLM들을 평가해봤고 전반적으로 성능이 좋지 않지만 NegCLIP이 괜찮아 보이는 결과를 냈습니다.

그래서 NegCLIP의 loss를 첨가해서 CLIP을 데이터셋에 튜닝하는 것으로 성능 향상을 관찰했네요. VLM 쪽에 새로운 데이터가 필요하다는 것을 강력하게 시사하는 듯 합니다. 이미 다들 같은 생각이겠지만요.

#vision-language #clip #dataset 