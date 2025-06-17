https://arxiv.org/abs/2406.17312

*Not All Preference Pairs Are Created Equal: A Recipe for Annotation-Efficient Iterative Preference Learning* (Sen Yang, Leyang Cui, Deng Cai, Xinting Huang, Shuming Shi, Wai Lam)

> Iterative preference learning, though yielding superior performances, requires online annotated preference labels. In this work, we study strategies to select worth-annotating response pairs for cost-efficient annotation while achieving competitive or even better performances compared with the random selection baseline for iterative preference learning. Built on assumptions regarding uncertainty and distribution shifts, we propose a comparative view to rank the implicit reward margins as predicted by DPO to select the response pairs that yield more benefits. Through extensive experiments, we show that annotating those response pairs with small margins is generally better than large or random, under both single- and multi-iteration scenarios. Besides, our empirical results suggest allocating more annotation budgets in the earlier iterations rather than later across multiple iterations.

DPO의 마진을 사용해서 어노테이션할 샘플을 고르는 문제. 여기서 흥미로운 것은 프롬프트-응답 페어들 중에서 샘플을 고르는 것 뿐만 아니라 응답을 N개 생성한 다음 어노테이션할 응답 페어 2개를 고르는 시도도 해봤다는 것이네요.

#active-learning #rlhf 