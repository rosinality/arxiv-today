https://arxiv.org/abs/2405.15613

*Automatic Data Curation for Self-Supervised Learning: A Clustering-Based Approach* (Huy V. Vo, Vasil Khalidov, Timothée Darcet, Théo Moutakanni, Nikita Smetanin, Marc Szafraniec, Hugo Touvron, Camille Couprie, Maxime Oquab, Armand Joulin, Hervé Jégou, Patrick Labatut, Piotr Bojanowski)

> Self-supervised features are the cornerstone of modern machine learning systems. They are typically pre-trained on data collections whose construction and curation typically require extensive human effort. This manual process has some limitations similar to those encountered in supervised learning, e.g., the crowd-sourced selection of data is costly and time-consuming, preventing scaling the dataset size. In this work, we consider the problem of automatic curation of high-quality datasets for self-supervised pre-training. We posit that such datasets should be large, diverse and balanced, and propose a clustering-based approach for building ones satisfying all these criteria. Our method involves successive and hierarchical applications of $k$-means on a large and diverse data repository to obtain clusters that distribute uniformly among data concepts, followed by a hierarchical, balanced sampling step from these clusters. Extensive experiments on three different data domains including web-based images, satellite images and text show that features trained on our automatically curated datasets outperform those trained on uncurated data while being on par or better than ones trained on manually curated data.

Self Supervised Learning을 위한 데이터셋은 크고 다양하며 균형이 잡혀 있어야 한다, 즉 특정한 컨셉이 지나치게 많은 비중을 차지해서는 안 된다는 가정 하에서 균형을 어떻게 맞출 것인가에 대한 문제입니다.

클러스터링을 한 다음 각 클러스터에서 고정된 숫자의 샘플을 뽑는다는 것이 바로 생각할 수 있는 방법이지만 균형이 깨진 데이터셋에 대해서는 K-means 같은 경우 같은 컨셉의 클러스터가 여러 개 발생하는 문제가 있죠. 그래서 반복적으로 K-means를 사용해 계층화된 클러스터를 만들고 이 클러스터 계층을 사용해 샘플링을 하는 방법을 사용했습니다.

Semantic Deduplication의 더 체계화된 방법이라고 할 수 있겠군요.

#dataset 