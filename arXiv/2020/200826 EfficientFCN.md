https://arxiv.org/abs/2008.10487
평소라면 보고 지나쳤을지도 모르겠는데 요즘 semantic segmentation이 필요한 문제가 생겨서 눈에 들어왔다.
semantic segmentation에서 작은 stride의 feature가 필요하다는 문제를 태클하는 방법으로는 u-net/fpn 같이 여러 stride의 feature를 결합하는 방법과 dilated backbone을 사용해서 stride 자체를 줄여버리는 방법이 대표적일 것이다.
요즘 논문으로 나오는 방법의 대세는 dilated backbone을 사용하는 방법이기는 하다. 다만 stride를 줄이고 그걸 dilated convolution으로 채우는 방식이니 그만큼 느리다. u-net/fpn과 같은 방법은 그 자체로는 global한 구조나 정보를 반영하는 메커니즘이 부족하다는 것이 논문의 요점이다.
그렇다면? u-net/fpn처럼 backbone의 stride는 그대로 놓고 global한 정보를 모델링하는 모듈을 붙여 그 부분을 보강하면 된다. 이 모듈의 구조가 핵심인데 전반적인 구조는 object-contextual representation(https://arxiv.org/abs/1909.11065)과 흡사한 감이 있다. 즉 feature들을 끌어모아 global한 정보를 반영하는 임베딩(혹은 일종의 semantic token)을 만들고(대충 attention 썼다는 뜻 ㅎ) 각 feature map에 대해 이 임베딩을 다시 적절하게 결합해서(이것도 대충 attention 썼다는 뜻 ㅎ) prediction에 활용하는 것이 요점이라고 할 수 있겠다. object-contextual representation과 다른 점으로는 이 semantic token을 만드는 과정에 supervision을 주는 대신 알아서 학습하도록 만들었다는 것과, stride를 줄이지 않기 때문에 feature map을 up/downsampling해서 크기를 맞춰서 활용한다는 것이 주요하겠다.
supervision을 주는 과정이 빠져서 좀 더 심플해지기도 했고 향상된 효율성을 고려할 때 성능도 나쁘지 않게 찍힌 것 같다. 비교가 더 다양한 데이터셋과 모델에 대해 이뤄졌으면 좋겠다 싶기는 한데.

#semantic_segmentation

# Links

[[200122 Object Contextual Representations.md]]