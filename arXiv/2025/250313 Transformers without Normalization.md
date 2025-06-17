https://arxiv.org/abs/2503.10622

*Transformers without Normalization* (Jiachen Zhu, Xinlei Chen, Kaiming He, Yann LeCun, Zhuang Liu)

> Normalization layers are ubiquitous in modern neural networks and have long been considered essential. This work demonstrates that Transformers without normalization can achieve the same or better performance using a remarkably simple technique. We introduce Dynamic Tanh (DyT), an element-wise operation $DyT($x$) = \tanh(\alpha $x$)$, as a drop-in replacement for normalization layers in Transformers. DyT is inspired by the observation that layer normalization in Transformers often produces tanh-like, $S$-shaped input-output mappings. By incorporating DyT, Transformers without normalization can match or exceed the performance of their normalized counterparts, mostly without hyperparameter tuning. We validate the effectiveness of Transformers with DyT across diverse settings, ranging from recognition to generation, supervised to self-supervised learning, and computer vision to language models. These findings challenge the conventional understanding that normalization layers are indispensable in modern neural networks, and offer new insights into their role in deep networks.

Layer Norm을 Tanh로 교체한 형태의 Norm Free Network군요. 최대값을 Bound하는 것만으로도 학습에 충분하다는 의미일 수 있겠네요.

Norm Free Network의 사례들은 Norm을 사용한 경우와 결과가 거의 같다는 것이 오히려 흥미롭습니다. Post Norm 같은 사례들을 생각하면 Norm의 여부 자체보다는 Norm을 어떻게 배치하는지가 더 영향이 큰 것 같네요.

Norm free network that replaces layer norm with tanh. This suggests that simply bounding the maximum values maybe sufficient for training.

What's particulary interesting about norm free network is their performance matches that of networks with normalization. When we consider examples like post norm, it seems that how we position the normalization matters more than whether we use normalization at all.

#normalization 