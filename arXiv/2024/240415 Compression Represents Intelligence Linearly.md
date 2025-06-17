https://arxiv.org/abs/2404.09937

*Compression Represents Intelligence Linearly* (Yuzhen Huang, Jinghan Zhang, Zifei Shan, Junxian He)

> There is a belief that learning to compress well will lead to intelligence. Recently, language modeling has been shown to be equivalent to compression, which offers a compelling rationale for the success of large language models (LLMs): the development of more advanced language models is essentially enhancing compression which facilitates intelligence. Despite such appealing discussions, little empirical evidence is present for the interplay between compression and intelligence. In this work, we examine their relationship in the context of LLMs, treating LLMs as data compressors. Given the abstract concept of "intelligence", we adopt the average downstream benchmark scores as a surrogate, specifically targeting intelligence related to knowledge and commonsense, coding, and mathematical reasoning. Across 12 benchmarks, our study brings together 30 public LLMs that originate from diverse organizations. Remarkably, we find that LLMs' intelligence -- reflected by average benchmark scores -- almost linearly correlates with their ability to compress external text corpora. These results provide concrete evidence supporting the belief that superior compression indicates greater intelligence. Furthermore, our findings suggest that compression efficiency, as an unsupervised metric derived from raw text corpora, serves as a reliable evaluation measure that is linearly associated with the model capabilities. We open-source our compression datasets as well as our data collection pipelines to facilitate future researchers to assess compression properly.

Bits Per Character와 벤치마크 성능에 대한 관계 추정. Common Crawl, GitHub, arXiv 코퍼스에서 BPC를 측정했습니다. 상관계수가 0.9 수준으로 잘 나옵니다.

코퍼스와 벤치마크를 다르게 한 경우나 코퍼스를 믹스한 경우에 대한 결과도 재미있네요. 서적 코퍼스에 대해 MMLU와의 상관계수가 더 높게 나왔다는 것도 흥미로운 결과입니다.

이 결과를 사용해 데이터셋을 구성하는 지침으로 사용할 수 있지 않을까 하는 생각도 드네요. 벤치마크와의 상관계수를 높이는 형태로 데이터셋을 전처리하거나 믹스할 수 있지 않을까 싶습니다.

#llm #dataset 