https://arxiv.org/abs/2308.08998

Reinforced Self-Training (ReST) for Language Modeling (Caglar Gulcehre, Tom Le Paine, Srivatsan Srinivasan, Ksenia Konyushkova, Lotte Weerts, Abhishek Sharma, Aditya Siddhant, Alex Ahern, Miaosen Wang, Chenjie Gu, Wolfgang Macherey, Arnaud Doucet, Orhan Firat, Nando de Freitas)

구글 딥마인드의 Alignment 알고리즘. 기본적으로는 rejection sampling과 비슷하게 샘플링을 한 다음 reward score로 필터링하고 필터링된 데이터셋으로 학습하는 방식입니다. 차이가 있다면 필터링 기준을 높여가면서 iterative하게 한다는 것과 학습 loss를 cross entropy 외에도 다른 offline rl loss를 고려했다는 것이겠네요.

테스트를 기계 번역에 대해 했다는 것도 재미있네요. 기계 번역에 preference modeling이 필요하다는 것을 보여주는 사례가 아닐지.

#alignment