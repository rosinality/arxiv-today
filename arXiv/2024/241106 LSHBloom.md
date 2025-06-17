https://arxiv.org/abs/2411.04257

*LSHBloom: Memory-efficient, Extreme-scale Document Deduplication* (Arham Khan, Robert Underwood, Carlo Siebenschuh, Yadu Babuji, Aswathy Ajith, Kyle Hippe, Ozan Gokdemir, Alexander Brace, Kyle Chard, Ian Foster)

> Deduplication is a major focus for assembling and curating training datasets for large language models (LLM) -- detecting and eliminating additional instances of the same content -- in large collections of technical documents. Unrestrained, duplicates in the training dataset increase training costs and lead to undesirable properties such as memorization in trained models or cheating on evaluation. Contemporary approaches to document-level deduplication are often extremely expensive in both runtime and memory. We propose LSHBloom, an extension to MinhashLSH, which replaces the expensive LSHIndex with lightweight Bloom filters. LSHBloom demonstrates the same deduplication performance as MinhashLSH with only a marginal increase in false positives (as low as 1e-5 in our experiments); demonstrates competitive runtime (270\% faster than MinhashLSH on peS2o); and, crucially, uses just 0.6\% of the disk space required by MinhashLSH to deduplicate peS2o. We demonstrate that this space advantage scales with increased dataset size -- at the extreme scale of several billion documents, LSHBloom promises a 250\% speedup and a 54$\times$ space advantage over traditional MinHashLSH scaling deduplication of text datasets to many billions of documents.

효율적인 Deduplication을 위한 방법. MinHashLSH의 Signature Matrix의 밴드들을 블룸 필터로 대체한 방법이군요. 프리트레이닝 코퍼스는 비용이 더 들더라도 조금이라도 나은 방법을 쓸 것 같기도 하지만...FineWeb이나 DCLM의 경우에도 Deduplication 부분에서 효율성을 위한 타협을 했었죠.

<english>
Method for efficient deduplication. Replacing bands of signature matrix of MinHashLSH into bloom filters. It may seem to natural to use most accurate method to preprocess pretraining corpus even it takes more costs, but even FineWeb or DCLM have made compromise for efficiency in deduplication.
</english>

#corpus 