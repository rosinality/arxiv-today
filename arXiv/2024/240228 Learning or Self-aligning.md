https://arxiv.org/abs/2402.18243

*Learning or Self-aligning? Rethinking Instruction Fine-tuning* (Mengjie Ren, Boxi Cao, Hongyu Lin, Liu Cao, Xianpei Han, Ke Zeng, Guanglu Wan, Xunliang Cai, Le Sun)

> Instruction Fine-tuning~(IFT) is a critical phase in building large language models~(LLMs). Previous works mainly focus on the IFT's role in the transfer of behavioral norms and the learning of additional world knowledge. However, the understanding of the underlying mechanisms of IFT remains significantly limited. In this paper, we design a knowledge intervention framework to decouple the potential underlying factors of IFT, thereby enabling individual analysis of different factors. Surprisingly, our experiments reveal that attempting to learn additional world knowledge through IFT often struggles to yield positive impacts and can even lead to markedly negative effects. Further, we discover that maintaining internal knowledge consistency before and after IFT is a critical factor for achieving successful IFT. Our findings reveal the underlying mechanisms of IFT and provide robust support for some very recent and potential future works.

Instruction Tuning의 반복되는 주제인 지식을 주입하는 것인가 혹은 가진 지식을 꺼내는 것인가라는 주제에 대한 탐색. Instruction Tuning 데이터셋을 나눠 1. 모델이 가진 지식과 일치하는 경우 2. 모델이 가진 지식과 불일치하는 경우 3. 모델이 가진 지식과 불일치하는 경우의 데이터셋에서 응답을 모델의 지식과 일치하도록 수정한 경우 세 가지를 가지고 분석합니다. 3의 경우에는 오답만 들어있게 되죠.

그런데 놀랍게도 2보다 3에서 나은 성능이 나타납니다. 즉 모델이 가진 지식을 바꾸려고 하면 성능이 낮아진다는 것이죠. 추가적인 분석을 통해 모델이 Instruction Tuning 이전과 이후에 갖고 있는 지식이 얼마나 일관된 지가 성능에 중요하다는 이야기를 합니다. 그런 의미에서는 3도 확실하게 갖고 있지 않던 지식을 반대 방향으로 강화시키기에 문제를 발생시킨다는 이야기를 하네요.

모델이 가진 지식과 부합한다는 것과 부합하지 않는다는 것을 분리하는 것이 까다로운 일이라 더 깊게 검토해봐야겠지만 흥미로운 주장인 것 같습니다. Instruction Tuning은 행동 방식만 바꾼다는 것을 넘어 행동 방식만 바꿀 때에야 최적이라는 아이디어일 수 있겠네요.

#instruction-tuning 