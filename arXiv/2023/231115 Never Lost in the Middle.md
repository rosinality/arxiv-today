https://arxiv.org/abs/2311.09198

Never Lost in the Middle: Improving Large Language Models via Attention Strengthening Question Answering (He Junqing, Pan Kunhao, Dong Xiaoqun, Song Zhuoyang, Liu Yibo, Liang Yuxin, Wang Hao, Sun Qianguo, Zhang Songxin, Xie Zejian, Zhang Jiaxing)

long context 상황에서 발생하는 lost in the middle 현상에 대한 대처. 중요한 포인트는 attention weight 자체가 주로 instruction이 있는 앞쪽과 뒤쪽에 쏠리고 있고, 중간 부분에 attention weight가 그다지 주어지지 않다 보니 lost in the middle이 발생하는 것이 자연스러울 수 있다는 부분일 듯 싶네요.

이 논문에서는 임의로 negative 문서를 추가해서 채워넣는 방식으로 QA 과제를 만들어서 학습시키는 방법으로 이 문제를 해소할 수 있었다고 제안합니다. 문제를 풀기 위해 문제에 직접 튜닝했다는 느낌이긴 합니다. 다만 lost in the middle을 테스트하는데 사용하는 형태의 데이터가 instruction tuning 과정에서 없을 수 있겠다는 것과 (그래서 long context 성능의 한계를 포착하는 것에는 한계가 있을 수 있다는 것), long context 과제를 위한 instruction tuning이 필요하겠다는 생각이 드네요.

#long_context 