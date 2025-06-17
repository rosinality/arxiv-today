https://arxiv.org/abs/2504.01801

*Investigating and Scaling up Code-Switching for Multilingual Language Model Pre-Training* (Zhijun Wang, Jiahuan Li, Hao Zhou, Rongxiang Weng, Jingang Wang, Xin Huang, Xue Han, Junlan Feng, Chao Deng, Shujian Huang)

> Large language models (LLMs) exhibit remarkable multilingual capabilities despite the extreme language imbalance in the pre-training data. In this paper, we closely examine the reasons behind this phenomenon, focusing on the pre-training corpus. We find that the existence of code-switching, alternating between different languages within a context, is key to multilingual capabilities. We conduct an analysis to investigate code-switching in the pre-training corpus, examining its presence and categorizing it into four types within two quadrants. We then assess its impact on multilingual performance. These types of code-switching data are unbalanced in proportions and demonstrate different effects on facilitating language transfer. To better explore the power of code-switching for language alignment during pre-training, we investigate the strategy of synthetic code-switching. We continuously scale up the synthetic code-switching data and observe remarkable improvements in both benchmarks and representation space. Extensive experiments indicate that incorporating synthetic code-switching data enables better language alignment and generalizes well to high, medium, and low-resource languages with pre-training corpora of varying qualities.

여러 패턴의 Code Switching 데이터를 사용한 Multilingual 성능의 향상 분석. 흥미롭게도 원문과 번역문을 같이 학습시키는 것보다는 아예 번역문으로 대체해버리는 것이 더 효과가 좋았다고 하는군요. 대체의 단위를 어떻게 해야 하는가에는 각 언어의 비율이 영향을 미치는 것 같군요.

<english>
Analysis on improvement of multilingual capabilities when using code switching data with various patterns. Interestingly they insist it is more effective to replace into translated texts instead of training both on original and translated texts. And it seems proportion of each language affects how the unit of replacement should be.
</english>

#multilingual #synthetic-data #pretraining 