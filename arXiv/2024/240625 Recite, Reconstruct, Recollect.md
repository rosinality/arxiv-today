https://arxiv.org/abs/2406.17746

*Recite, Reconstruct, Recollect: Memorization in LMs as a Multifaceted Phenomenon* (USVSN Sai Prashanth, Alvin Deng, Kyle O'Brien, Jyothir S V, Mohammad Aflah Khan, Jaydeep Borkar, Christopher A. Choquette-Choo, Jacob Ray Fuehne, Stella Biderman, Tracy Ke, Katherine Lee, Naomi Saphra)

> Memorization in language models is typically treated as a homogenous phenomenon, neglecting the specifics of the memorized data. We instead model memorization as the effect of a set of complex factors that describe each sample and relate it to the model and corpus. To build intuition around these factors, we break memorization down into a taxonomy: recitation of highly duplicated sequences, reconstruction of inherently predictable sequences, and recollection of sequences that are neither. We demonstrate the usefulness of our taxonomy by using it to construct a predictive model for memorization. By analyzing dependencies and inspecting the weights of the predictive model, we find that different factors influence the likelihood of memorization differently depending on the taxonomic category.

LLM의 Memorization에 대한 분석. 일단 k-extractable이라고 해서 k개 토큰을 프롬프트로 주면 이후 k개의 토큰을 그대로 생성할 수 있는 사례에 대해 분석합니다. 이 상황에서 Memorization을 다음과 같이 분류하네요.

1. Recitation. 프리트레이닝 코퍼스에 6회 이상 등장한 텍스트인 경우.
2. Reconstruction. 템플릿이 있어 그 템플릿을 활용한 경우. (예를 들어 번호를 계속 증가시키는 등) 이쪽은 Memorization이라고 하기에는 거리가 있죠.
3. Recollection. Recitation과 Reconstruction이 아닌 경우.

이 분류에 따라 모델의 학습 과정에 따라 각 분류가 학습되는 패턴의 변화, 그리고 텍스트의 특성에 따라 각 분류의 Memorization이 일어나는 확률이 어떻게 변화하는지를 분석했습니다. 결과적으로 세 가지 Memorization이 서로 다른 메커니즘으로 발생한다는 것을 시사한다고 생각할 수 있겠네요.

#llm 