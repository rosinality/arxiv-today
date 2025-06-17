https://arxiv.org/abs/2409.07431

*Synthetic continued pretraining* (Zitong Yang, Neil Band, Shuangping Li, Emmanuel Candès, Tatsunori Hashimoto)

> Pretraining on large-scale, unstructured internet text has enabled language models to acquire a significant amount of world knowledge. However, this knowledge acquisition is data-inefficient -- to learn a given fact, models must be trained on hundreds to thousands of diverse representations of it. This poses a challenge when adapting a pretrained model to a small corpus of domain-specific documents, where each fact may appear rarely or only once. We propose to bridge this gap with synthetic continued pretraining: using the small domain-specific corpus to synthesize a large corpus more amenable to learning, and then performing continued pretraining on the synthesized corpus. We instantiate this proposal with EntiGraph, a synthetic data augmentation algorithm that extracts salient entities from the source documents and then generates diverse text by drawing connections between the sampled entities. Synthetic continued pretraining using EntiGraph enables a language model to answer questions and follow generic instructions related to the source documents without access to them. If instead, the source documents are available at inference time, we show that the knowledge acquired through our approach compounds with retrieval-augmented generation. To better understand these results, we build a simple mathematical model of EntiGraph, and show how synthetic data augmentation can "rearrange" knowledge to enable more data-efficient learning.

합성 데이터를 사용해 데이터를 증폭하여 데이터 규모가 작은 도메인에 대해 Continual Pretraining. 엔티티를 추출하고 엔티티에 대한 설명, 그리고 엔티티들 사이의 관계에 대한 설명들을 생성하고 이 텍스트를 학습 데이터로 사용했네요.

그렇다면 이를 작은 도메인이 아니라 전체 프리트레이닝 데이터에 대해 한다면이라는 생각을 해보게 되죠.

기본적으로 Phi 시리즈 같은 시도를 연상할 수 있겠네요. Phi를 어떻게 생각할 것인가 하는 것은 중요한 문제이긴 합니다. 다만 한 가지, 사람이 생성한 데이터를 중요하게 생각해야 한다는 것과 합성 데이터를 그 데이터에 대해서 더 잘 학습하기 위한 방법으로서 생각하면 조금 갈피가 되지 않을까 싶습니다.

#synthetic-data #continual-pretraining