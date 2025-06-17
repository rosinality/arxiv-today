https://arxiv.org/abs/2412.03398

*RedStone: Curating General, Code, Math, and QA Data for Large Language Models* (Yaoyao Chang, Lei Cui, Li Dong, Shaohan Huang, Yangyu Huang, Yupan Huang, Scarlett Li, Tengchao Lv, Shuming Ma, Qinzheng Sun, Wenhui Wang, Furu Wei, Ying Xin, Mao Yang, Qiufeng Yin, Xingxing Zhang)

> Pre-training Large Language Models (LLMs) on high-quality, meticulously curated datasets is widely recognized as critical for enhancing their performance and generalization capabilities. This study explores the untapped potential of Common Crawl as a comprehensive and flexible resource for pre-training LLMs, addressing both general-purpose language understanding and specialized domain knowledge. We introduce RedStone, an innovative and scalable pipeline engineered to extract and process data from Common Crawl, facilitating the creation of extensive and varied pre-training datasets. Unlike traditional datasets, which often require expensive curation and domain-specific expertise, RedStone leverages the breadth of Common Crawl to deliver datasets tailored to a wide array of domains. In this work, we exemplify its capability by constructing pre-training datasets across multiple fields, including general language understanding, code, mathematics, and question-answering tasks. The flexibility of RedStone allows for easy adaptation to other specialized domains, significantly lowering the barrier to creating valuable domain-specific datasets. Our findings demonstrate that Common Crawl, when harnessed through effective pipelines like RedStone, can serve as a rich, renewable source of pre-training data, unlocking new avenues for domain adaptation and knowledge discovery in LLMs. This work also underscores the importance of innovative data acquisition strategies and highlights the role of web-scale data as a powerful resource in the continued evolution of LLMs. RedStone code and data samples will be publicly available at \url{https://aka.ms/redstone}.

마이크로소프트의 프리트레이닝 코퍼스. Common Crawl에 대한 처리는 기본적인 스타일인데 WARC와 WET 각각에 대해서 했다는 게 좀 특이하네요. 추가적으로 수학, 코드 데이터 수집에 더해 QA 데이터 수집을 따로 했군요.

<english>
Pretraining corpus from Microsoft. On Common Crawl they employed common method of processing but it is unusual that they did it on both WARC and WET. Additionally they have collected mathematics and code related texts, along with QA.
</english>

#pretraining #corpus 