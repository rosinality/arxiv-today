https://arxiv.org/abs/2506.21545

*Data Efficacy for Language Model Training* (Yalun Dai, Yangyu Huang, Xin Zhang, Wenshan Wu, Chong Li, Wenhui Lu, Shijie Cao, Li Dong, Scarlett Li)

> Data is fundamental to the training of language models (LM). Recent research has been dedicated to data efficiency, which aims to maximize performance by selecting a minimal or optimal subset of training data. Techniques such as data filtering, sampling, and selection play a crucial role in this area. To complement it, we define Data Efficacy, which focuses on maximizing performance by optimizing the organization of training data and remains relatively underexplored. This work introduces a general paradigm, DELT, for considering data efficacy in LM training, which highlights the significance of training data organization. DELT comprises three components: Data Scoring, Data Selection, and Data Ordering. Among these components, we design Learnability-Quality Scoring (LQS), as a new instance of Data Scoring, which considers both the learnability and quality of each data sample from the gradient consistency perspective. We also devise Folding Ordering (FO), as a novel instance of Data Ordering, which addresses issues such as model forgetting and data distribution bias. Comprehensive experiments validate the data efficacy in LM training, which demonstrates the following: Firstly, various instances of the proposed DELT enhance LM performance to varying degrees without increasing the data scale and model size. Secondly, among these instances, the combination of our proposed LQS for data scoring and Folding for data ordering achieves the most significant improvement. Lastly, data efficacy can be achieved together with data efficiency by applying data selection. Therefore, we believe that data efficacy is a promising foundational area in LM training.

LLM 학습의 데이터 Efficacy. Efficiency와는 다르게 같은 데이터의 재배치를 통해서 성능을 높인다는 관점. 여기서는 Folding이라는, 커리큘럼을 여러 번 반복하는 방법을 시도했군요.

같은 데이터에서 더 많은 것을 학습하는 방법은 앞으로 더더욱 중요한 문제겠죠.

<english>
Data efficacy for LLM training. In contrast of efficiency, it is a viewpoint of enhancing performance by reordering of same data. This works tried a method of folding, which repeats same curriculum multiple times.

I think the method to train a model more from same data would become more and more crucial.
</english>

#pretraining #llm 