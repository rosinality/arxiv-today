https://arxiv.org/abs/2404.07177

*Scaling Laws for Data Filtering -- Data Curation cannot be Compute Agnostic* (Sachin Goyal, Pratyush Maini, Zachary C. Lipton, Aditi Raghunathan, J. Zico Kolter)

> Vision-language models (VLMs) are trained for thousands of GPU hours on carefully curated web datasets. In recent times, data curation has gained prominence with several works developing strategies to retain 'high-quality' subsets of 'raw' scraped data. For instance, the LAION public dataset retained only 10% of the total crawled data. However, these strategies are typically developed agnostic of the available compute for training. In this paper, we first demonstrate that making filtering decisions independent of training compute is often suboptimal: the limited high-quality data rapidly loses its utility when repeated, eventually requiring the inclusion of 'unseen' but 'lower-quality' data. To address this quality-quantity tradeoff ($\texttt{QQT}$), we introduce neural scaling laws that account for the non-homogeneous nature of web data, an angle ignored in existing literature. Our scaling laws (i) characterize the $\textit{differing}$ 'utility' of various quality subsets of web data; (ii) account for how utility diminishes for a data point at its 'nth' repetition; and (iii) formulate the mutual interaction of various data pools when combined, enabling the estimation of model performance on a combination of multiple data pools without ever jointly training on them. Our key message is that data curation $\textit{cannot}$ be agnostic of the total compute that a model will be trained for. Our scaling laws allow us to curate the best possible pool for achieving top performance on Datacomp at various compute budgets, carving out a pareto-frontier for data curation. Code is available at https://github.com/locuslab/scaling_laws_data_filtering.

고퀄리티 데이터를 Multi Epoch 학습시키기 vs 낮은 퀄리티 데이터도 포함해서 1 Epoch 학습시키기라는 중요한 문제에 대한 탐색이네요. 총 학습량이 작을 때는 높은 퀄리티의 데이터만 쓰는 쪽이 낫고 학습량이 늘어날수록 낮은 퀄리티 데이터도 포함하는 쪽이 낫습니다. DeepSeek LLM (https://arxiv.org/abs/2401.02954) 에서 데이터의 퀄리티가 높아짐에 따라 모델 크기에 대한 Exponent가 증가했던 결과와 연결되는 결과인 것 같습니다.

아주 쓸모 없는 데이터가 아니라면 데이터를 필터링하는 것보다는 샘플의 퀄리티를 개선하기 위한 작업을 하는 쪽이 나을 수 있겠다는 생각이 드네요. 물론 주어진 연산량에서 최적 지점을 찾기 위한 Scaling Law 탐색을 먼저 해야겠지만요.

#scaling-law

# Links

[[240105 DeepSeek LLM.md]]