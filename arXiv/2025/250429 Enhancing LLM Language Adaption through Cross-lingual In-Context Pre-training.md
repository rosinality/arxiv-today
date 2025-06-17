https://arxiv.org/abs/2504.20484

*Enhancing LLM Language Adaption through Cross-lingual In-Context Pre-training* (Linjuan Wu, Haoran Wei, Huan Lin, Tianhao Li, Baosong Yang, Weiming Lu)

> Large language models (LLMs) exhibit remarkable multilingual capabilities despite English-dominated pre-training, attributed to cross-lingual mechanisms during pre-training. Existing methods for enhancing cross-lingual transfer remain constrained by parallel resources, suffering from limited linguistic and domain coverage. We propose Cross-lingual In-context Pre-training (CrossIC-PT), a simple and scalable approach that enhances cross-lingual transfer by leveraging semantically related bilingual texts via simple next-word prediction. We construct CrossIC-PT samples by interleaving semantic-related bilingual Wikipedia documents into a single context window. To access window size constraints, we implement a systematic segmentation policy to split long bilingual document pairs into chunks while adjusting the sliding window mechanism to preserve contextual coherence. We further extend data availability through a semantic retrieval framework to construct CrossIC-PT samples from web-crawled corpus. Experimental results demonstrate that CrossIC-PT improves multilingual performance on three models (Llama-3.1-8B, Qwen2.5-7B, and Qwen2.5-1.5B) across six target languages, yielding performance gains of 3.79%, 3.99%, and 1.95%, respectively, with additional improvements after data augmentation.

위키피디아의 다국어 문서들을 연결해서 다국어 프리트레이닝 데이터를 구축. 위키피디아의 경우에는 거의 번역 관계인 경우가 많긴 할 텐데, 번역을 넘어 의미적으로 연관된 다국어 문서들을 결합하면 어떻게 될지 궁금하네요.

<english>
Constructing multilingual pretraining data by connecting multilingual documents in wikipeida. In wikipedia many of documents are tranlsations of each others. But I wounder what result we can get if we combines semantically related multilingual documents beyond translations.
</english>

#multilingual #pretraining 