https://arxiv.org/abs/2410.02660

*How to Train Long-Context Language Models (Effectively)* (Tianyu Gao, Alexander Wettig, Howard Yen, Danqi Chen)

> We study continued training and supervised fine-tuning (SFT) of a language model (LM) to make effective use of long-context information. We first establish a reliable evaluation protocol to guide model development -- Instead of perplexity or simple needle-in-a-haystack (NIAH) tests, we use a broad set of long-context tasks, and we evaluate models after SFT with instruction data as this better reveals long-context abilities. Supported by our robust evaluations, we run thorough experiments to decide the data mix for continued pre-training, the instruction tuning dataset, and many other design choices. We find that (1) code repositories and books are excellent sources of long data, but it is crucial to combine them with high-quality short data; (2) training with a sequence length beyond the evaluation length boosts long-context performance; (3) for SFT, using only short instruction datasets yields strong performance on long-context tasks. Our final model, ProLong-8B, which is initialized from Llama-3 and trained on 40B tokens, demonstrates state-of-the-art long-context performance among similarly sized models at a length of 128K. ProLong outperforms Llama-3.18B-Instruct on the majority of long-context tasks despite having seen only 5% as many tokens during long-context training. Additionally, ProLong can effectively process up to 512K tokens, one of the longest context windows of publicly available LMs.

Long Context 튜닝 레시피. 짧은 데이터를 섞은 긴 텍스트들을 준비하고, 오래, 평가 시점보다 더 긴 길이에 대해 튜닝하는 것이 좋다는 결론.

<english>
Recipes for long context tuning. Mixing long texts with short texts, and do longer training on longer contexts larger than which is used at evaluation time.
</english>

#long-context 