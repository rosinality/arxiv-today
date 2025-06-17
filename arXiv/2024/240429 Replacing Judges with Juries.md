https://arxiv.org/abs/2404.18796

*Replacing Judges with Juries: Evaluating LLM Generations with a Panel of Diverse Models* (Pat Verga, Sebastian Hofstatter, Sophia Althammer, Yixuan Su, Aleksandra Piktus, Arkady Arkhangorodsky, Minjie Xu, Naomi White, Patrick Lewis)

> As Large Language Models (LLMs) have become more advanced, they have outpaced our abilities to accurately evaluate their quality. Not only is finding data to adequately probe particular model properties difficult, but evaluating the correctness of a model's freeform generation alone is a challenge. To address this, many evaluations now rely on using LLMs themselves as judges to score the quality of outputs from other LLMs. Evaluations most commonly use a single large model like GPT4. While this method has grown in popularity, it is costly, has been shown to introduce intramodel bias, and in this work, we find that very large models are often unnecessary. We propose instead to evaluate models using a Panel of LLm evaluators (PoLL). Across three distinct judge settings and spanning six different datasets, we find that using a PoLL composed of a larger number of smaller models outperforms a single large judge, exhibits less intra-model bias due to its composition of disjoint model families, and does so while being over seven times less expensive.

GPT-4 대신 저렴한 Haiku, Command R, GPT-3.5 같은 모델들을 여럿 사용해서 평가하는 방법. 결과적으로는 이쪽이 평가 성능도 더 높습니다. GPT-4의 평가 성능이 상당히 낮게 잡히고 있는 결과라는 점을 유의해야 할 것 같긴 합니다.

#evaluation 