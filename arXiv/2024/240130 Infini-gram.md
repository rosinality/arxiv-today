https://arxiv.org/abs/2401.17377

*Infini-gram: Scaling Unbounded n-gram Language Models to a Trillion Tokens* (Jiacheng Liu, Sewon Min, Luke Zettlemoyer, Yejin Choi, Hannaneh Hajishirzi)

> Are n-gram language models still relevant in this era of neural large language models (LLMs)? Our answer is yes, and we show their values in both text analysis and improving neural LLMs. Yet this necessitates modernizing n-gram models in two aspects. First, we train them at the same data scale as neural LLMs -- 1.4 trillion tokens. This is the largest n-gram model ever built. Second, existing n-gram models use small n which hinders their performance; we instead allow n to be arbitrarily large, by introducing a new $\infty$-gram LM with backoff. Instead of pre-computing n-gram count tables (which would be very expensive), we develop an engine named infini-gram -- powered by suffix arrays -- that can compute $\infty$-gram (as well as n-gram with arbitrary n) probabilities with millisecond-level latency. The $\infty$-gram framework and infini-gram engine enable us to conduct many novel and interesting analyses of human-written and machine-generated text: we find that the $\infty$-gram LM has fairly high accuracy for next-token prediction (47%), and can complement neural LLMs to greatly reduce their language modeling perplexities. When analyzing machine-generated text, we also observe irregularities in the machine--$\infty$-gram agreement level with respect to the suffix length, which indicates deficiencies in neural LLM pretraining and the positional embeddings of Transformers. We open-source our infini-gram engine in the hopes of enabling more study on how to best use verbatim information retrieved from large text corpora.

이거 재밌네요. 무한대 n을 허용하는 n-gram LM입니다. 결과적으로는 데이터셋에 등장하는 최대 길이의 프롬프트 suffix의 등장 횟수를 세는 문제가 됩니다. 이 논문의 핵심은 이걸 효율적으로 처리할 수 있는 시스템을 구축한 것이네요.

LLM과의 비교도 재미있습니다. LLM은 확률이 낮다고 예측하지만 n-gram LM에서는 꽤 높은 경우들이 보이네요. 데이터셋 탐색이나 처리에 쓸 수 있는 도구가 될 수 있지 않을까 싶습니다.

#lm #dataset 

n-gram LM that allows infinite n. Consequently, this turns problem into counting number of occurences of the longest suffix of prompt in the corpus. The main point of this study is processing and querying this efficiently.

Comparison with neural LM is interesting. There are cases that neural LM assigns low probability but contrastly neural LM agrees with human substantially. It maybe could be useful tools for dataset exploration or processing.