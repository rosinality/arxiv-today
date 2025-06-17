https://arxiv.org/abs/2409.09613

*Rethinking KenLM: Good and Bad Model Ensembles for Efficient Text Quality Filtering in Large Web Corpora* (Yungi Kim, Hyunsoo Ha, Sukyung Lee, Jihoo Kim, Seonghoon Yang, Chanjun Park)

> With the increasing demand for substantial amounts of high-quality data to train large language models (LLMs), efficiently filtering large web corpora has become a critical challenge. For this purpose, KenLM, a lightweight n-gram-based language model that operates on CPUs, is widely used. However, the traditional method of training KenLM utilizes only high-quality data and, consequently, does not explicitly learn the linguistic patterns of low-quality data. To address this issue, we propose an ensemble approach that leverages two contrasting KenLMs: (i) Good KenLM, trained on high-quality data; and (ii) Bad KenLM, trained on low-quality data. Experimental results demonstrate that our approach significantly reduces noisy content while preserving high-quality content compared to the traditional KenLM training method. This indicates that our method can be a practical solution with minimal computational overhead for resource-constrained environments.

n-gram LM을 사용한 필터링은 주로 Positive 셋에 대해 LM을 학습시킨 다음 Perplexity로 필터링하는 방법을 사용하죠. 여기서는 명시적으로 Negative 셋에 대해 LM을 학습시켜서 Perplexity의 차이를 측정하는 방법을 사용합니다.

LM Loss의 차이라는 점에서 Learnability와 (https://arxiv.org/abs/2404.07965, https://arxiv.org/abs/2408.08310) 연결할 수 있지 않을까 싶네요. 보통 학습하는 LM 혹은 작은 LM을 사용하는데 여기에 n-gram LM을 사용했다고 생각할 수 있지 않을까 싶습니다.

#corpus

# Links

[[240815 ScalingFilter.md]]
[[240411 Rho-1.md]]