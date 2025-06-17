https://arxiv.org/abs/2503.09799

*Communication-Efficient Language Model Training Scales Reliably and Robustly: Scaling Laws for DiLoCo* (Zachary Charles, Gabriel Teston, Lucio Dery, Keith Rush, Nova Fallen, Zachary Garrett, Arthur Szlam, Arthur Douillard)

> As we scale to more massive machine learning models, the frequent synchronization demands inherent in data-parallel approaches create significant slowdowns, posing a critical challenge to further scaling. Recent work develops an approach (DiLoCo) that relaxes synchronization demands without compromising model quality. However, these works do not carefully analyze how DiLoCo's behavior changes with model size. In this work, we study the scaling law behavior of DiLoCo when training LLMs under a fixed compute budget. We focus on how algorithmic factors, including number of model replicas, hyperparameters, and token budget affect training in ways that can be accurately predicted via scaling laws. We find that DiLoCo scales both predictably and robustly with model size. When well-tuned, DiLoCo scales better than data-parallel training with model size, and can outperform data-parallel training even at small model sizes. Our results showcase a more general set of benefits of DiLoCo than previously documented, including increased optimal batch sizes, improved downstream generalization with scale, and improved evaluation loss for a fixed token budget.

DiLoCo에 대한 Scaling Law. 학습 규모에 따라 Data Parallel과의 차이가 감소하고 심지어 더 나아지는 구간이 발생하네요. Local SGD에 대한 Scaling Law도 이전에 나왔었죠 (https://arxiv.org/abs/2409.13198). 

DiLoCo를 상당히 열심히 개발하고 있네요. 요즘처럼 기술이 기밀이 되는 시대에 계속해서 공개되고 있다는 것이 좀 더 수상하게(?) 만드는 것은 있습니다.

Scaling law for DiLoCo. As training scale increases, the performance gap with data parallel decreases, and there are even points where it surpasses. A scaling law for local SGD was also published previously (https://arxiv.org/abs/2409.13198).

DiLoCo is being developed quite intensively. Ironically, in an era where technologies are increasingly becoming trade secrets, the continued publication of DiLoCo makes it somewhat suspicious.

#efficient-training #scaling-law 