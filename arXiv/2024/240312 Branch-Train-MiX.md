https://arxiv.org/abs/2403.07816

*Branch-Train-MiX: Mixing Expert LLMs into a Mixture-of-Experts LLM* (Sainbayar Sukhbaatar, Olga Golovneva, Vasu Sharma, Hu Xu, Xi Victoria Lin, Baptiste Rozière, Jacob Kahn, Daniel Li, Wen-tau Yih, Jason Weston, Xian Li)

> We investigate efficient methods for training Large Language Models (LLMs) to possess capabilities in multiple specialized domains, such as coding, math reasoning and world knowledge. Our method, named Branch-Train-MiX (BTX), starts from a seed model, which is branched to train experts in embarrassingly parallel fashion with high throughput and reduced communication cost. After individual experts are asynchronously trained, BTX brings together their feedforward parameters as experts in Mixture-of-Expert (MoE) layers and averages the remaining parameters, followed by an MoE-finetuning stage to learn token-level routing. BTX generalizes two special cases, the Branch-Train-Merge method, which does not have the MoE finetuning stage to learn routing, and sparse upcycling, which omits the stage of training experts asynchronously. Compared to alternative approaches, BTX achieves the best accuracy-efficiency tradeoff.

Domain Expert를 학습한 다음에 이 Expert를 묶어 MoE 모델로 만듭니다. FFN은 MoE로 묶으면 되고 Self Attention은 그냥 평균을 내버리네요. 굳이 도메인 레이블 같은 것을 결합하진 않고 일반적인 토큰 기반 Routing 입니다.

Sparse Upcycling (https://arxiv.org/abs/2212.05055) 의 7B 규모 실험도 같이 나오게 됐네요. Sparse Upcycling과 비교하면 어떤가? 라는 문제에 대해서는 각 Domain Expert를 학습시키는 것은 (GPU만 넉넉하다면) 완전히 병렬적으로 할 수 있다는 점을 강조하고 있습니다.

#moe

# Links

