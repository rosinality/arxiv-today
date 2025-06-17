https://arxiv.org/abs/2403.18058

*COIG-CQIA: Quality is All You Need for Chinese Instruction Fine-tuning* (Yuelin Bai, Xinrun Du, Yiming Liang, Yonggang Jin, Ziqiang Liu, Junting Zhou, Tianyu Zheng, Xincheng Zhang, Nuo Ma, Zekun Wang, Ruibin Yuan, Haihong Wu, Hongquan Lin, Wenhao Huang, Jiajun Zhang, Wenhu Chen, Chenghua Lin, Jie Fu, Min Yang, Shiwen Ni, Ge Zhang)

> Recently, there have been significant advancements in large language models (LLMs), particularly focused on the English language. These advancements have enabled these LLMs to understand and execute complex instructions with unprecedented accuracy and fluency. However, despite these advancements, there remains a noticeable gap in the development of Chinese instruction tuning. The unique linguistic features and cultural depth of the Chinese language pose challenges for instruction tuning tasks. Existing datasets are either derived from English-centric LLMs or are ill-suited for aligning with the interaction patterns of real-world Chinese users. To bridge this gap, we introduce COIG-CQIA, a high-quality Chinese instruction tuning dataset. Our aim is to build a diverse, wide-ranging instruction-tuning dataset to better align model behavior with human interactions. To this end, we collect a high-quality human-written corpus from various sources on the Chinese Internet, including Q&A communities, Wikis, examinations, and existing NLP datasets. This corpus was rigorously filtered and carefully processed to form the COIG-CQIA dataset. Furthermore, we train models of various scales on different subsets of CQIA, following in-depth evaluation and analyses. The findings from our experiments offer valuable insights for selecting and developing Chinese instruction-tuning datasets. We also find that models trained on CQIA-Subset achieve competitive results in human assessment as well as knowledge and security benchmarks. Data are available at https://huggingface.co/datasets/m-a-p/COIG-CQIA

얼마 전에 나왔던 Instruction Data에서 퀄리티가 중요하다는 다소간 당연한 결과입니다만 여기서 만든 데이터셋을 구성하는 한 가지 데이터가 재미있네요. Ruo Zhi Ba라고 해서 쓸데 없는 질문들을 모아놓은 데이터셋이 있는데 이 데이터셋이 단독으로도 가장 의미있는 것으로 나타났습니다.

Ruo Zhi Ba 데이터셋의 질문들은 커피콩도 콩이니 커피도 두유인가 같은 중국식 말장난 같은 것들이 많다고 합니다. https://x.com/AlbertBoyangLi/status/1775901595089416509 프롬프트의 중요성에 관련된 사례일 것 같네요. 물론 (사람이 작성한 경우도 있긴 하지만) GPT-4 응답을 필터링해서 사용한 것이니 응답에 대한 편향도 있긴 합니다.

대략 이런 질문들이 있습니다.

질문: 사마의는 왜 세 명의 못난이를 데려다가 제갈량을 대항하지 않았나요?
답변: 이는 역사 속의 일화와 속담입니다. "세 명의 못난이가 제갈량을 당해낼 수 있다"는 속담의 진정한 의미는, 평범한 능력을 가진 세 사람이 함께한다면, 마음을 모아 협력하고 집단의 지혜를 모은다면 제갈량보다 더 완벽한 계략을 생각해낼 수도 있다는 것입니다. 주의해야 할 점은 여기서 "세 명"은 여러 사람을 의미하는 것이고, 여기서 "당하다"는 물리적으로 막는 것을 의미하지 않습니다.

#instruction-tuning 