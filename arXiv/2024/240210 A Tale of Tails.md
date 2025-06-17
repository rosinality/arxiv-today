https://arxiv.org/abs/2402.07043

*A Tale of Tails: Model Collapse as a Change of Scaling Laws* (Elvis Dohmatob, Yunzhen Feng, Pu Yang, Francois Charton, Julia Kempe)

> As AI model size grows, neural scaling laws have become a crucial tool to predict the improvements of large models when increasing capacity and the size of original (human or natural) training data. Yet, the widespread use of popular models means that the ecosystem of online data and text will co-evolve to progressively contain increased amounts of synthesized data. In this paper we ask: How will the scaling laws change in the inevitable regime where synthetic data makes its way into the training corpus? Will future models, still improve, or be doomed to degenerate up to total (model) collapse? We develop a theoretical framework of model collapse through the lens of scaling laws. We discover a wide range of decay phenomena, analyzing loss of scaling, shifted scaling with number of generations, the ''un-learning" of skills, and grokking when mixing human and synthesized data. Our theory is validated by large-scale experiments with a transformer on an arithmetic task and text generation using the large language model Llama2.

모델의 생성 데이터를 쓰는 것이 Scaling Law에 미칠 수 있는 문제. 생성 데이터는 필연적으로 데이터 분포의 꼬리를 잘라내게 되고, 이 꼬리가 잘려나가는 문제로 인해 Scaling Curve가 깨지고 Lower Bound가 생긴다는 분석.

분포의 꼬리가 잘려나간다는 것은 Scaling으로 인해 발생하는 새로운 능력에 제한이 걸릴 수 있다는 의미이고 이건 Scaling에 있어 아주 큰 문제가 되겠죠. 이 결과에 대한 함의에 대해서는 많이 생각해 봐야 할 것 같지만 일차적으로는 학습 분포에 대한 추가 샘플을 얻는 접근은 안 된다는 생각을 하게 되네요. 결국 Information Processing Inequality로 돌아가는 것 같긴 합니다만.

#synthetic-data #scaling-law 