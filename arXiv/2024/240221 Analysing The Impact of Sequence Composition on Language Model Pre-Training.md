https://arxiv.org/abs/2402.13991

*Analysing The Impact of Sequence Composition on Language Model Pre-Training* (Yu Zhao, Yuanbin Qu, Konrad Staniszewski, Szymon Tworkowski, Wei Liu, Piotr Miłoś, Yuxiang Wu, Pasquale Minervini)

> Most language model pre-training frameworks concatenate multiple documents into fixed-length sequences and use causal masking to compute the likelihood of each token given its context; this strategy is widely adopted due to its simplicity and efficiency. However, to this day, the influence of the pre-training sequence composition strategy on the generalisation properties of the model remains under-explored. In this work, we find that applying causal masking can lead to the inclusion of distracting information from previous documents during pre-training, which negatively impacts the performance of the models on language modelling and downstream tasks. In intra-document causal masking, the likelihood of each token is only conditioned on the previous tokens in the same document, eliminating potential distracting information from previous documents and significantly improving performance. Furthermore, we find that concatenating related documents can reduce some potential distractions during pre-training, and our proposed efficient retrieval-based sequence construction method, BM25Chunk, can improve in-context learning (+11.6\%), knowledge memorisation (+9.8\%), and context utilisation (+7.2\%) abilities of language models without sacrificing efficiency.

In-context Pretraining을 BM25로 구현. 그러나 문서 경계에 대해 Masking을 하는 쪽이 더 나은 선택.

#llm #pretraining 