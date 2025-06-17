https://arxiv.org/abs/2412.02595

*Nemotron-CC: Transforming Common Crawl into a Refined Long-Horizon Pretraining Dataset* (Dan Su, Kezhi Kong, Ying Lin, Joseph Jennings, Brandon Norick, Markus Kliegl, Mostofa Patwary, Mohammad Shoeybi, Bryan Catanzaro)

> Recent English Common Crawl datasets like FineWeb-Edu and DCLM achieved significant benchmark gains via aggressive model-based filtering, but at the cost of removing 90% of data. This limits their suitability for long token horizon training, such as 15T tokens for Llama 3.1. In this paper, we show how to achieve better trade-offs between accuracy and data quantity by a combination of classifier ensembling, synthetic data rephrasing, and reduced reliance on heuristic filters. When training 8B parameter models for 1T tokens, using a high-quality subset of our data improves MMLU by 5.6 over DCLM, demonstrating the efficacy of our methods for boosting accuracies over a relatively short token horizon. Furthermore, our full 6.3T token dataset matches DCLM on MMLU, but contains four times more unique real tokens than DCLM. This unlocks state-of-the-art training over a long token horizon: an 8B parameter model trained for 15T tokens, of which 7.2T came from our dataset, is better than the Llama 3.1 8B model: +5 on MMLU, +3.1 on ARC-Challenge, and +0.5 on average across ten diverse tasks. The dataset is available at https://data.commoncrawl.org/contrib/Nemotron/Nemotron-CC/index.html

NVIDIA의 프리트레이닝 코퍼스 구축 작업. Trafilatura 같은 Extractor가 추출되는 텍스트의 양을 줄이는 경향과 휴리스틱 필터가 텍스트를 지나치게 필터링하는 문제에 대응했군요. 모델 기반 퀄리티 필터링에 힘이 실리고 있습니다.

그리고 합성 데이터를 포함시켰고 Global Deduplication을 사용했군요. 프리트레이닝 코퍼스와 관련된 중요한 문제들을 확인해주는 결과입니다.

<english>
Work from NVIDIA on building pretraining corpus. They dealt with the problem of tendency to reducing the amount text of extractors like Trafilatura, and excessive filtering from heruistic rules. Model based quality filtering is gaining a lof of focus.

They also incorporated synthetic data and employed global deduplication. It is the result that reveals important problems related to pretraining corpus.
</english>

#corpus #pretraining 