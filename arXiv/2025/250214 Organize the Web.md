https://arxiv.org/abs/2502.10341

*Organize the Web: Constructing Domains Enhances Pre-Training Data Curation* (Alexander Wettig, Kyle Lo, Sewon Min, Hannaneh Hajishirzi, Danqi Chen, Luca Soldaini)

> Modern language models are trained on large, unstructured datasets consisting of trillions of tokens and obtained by crawling the web. The unstructured nature makes it difficult to reason about their contents and develop systematic approaches to data curation. In this paper, we unpack monolithic web corpora by developing taxonomies of their contents and organizing them into domains. We introduce WebOrganizer, a framework for organizing web pages in terms of both their topic and format. Using these two complementary notions of domains, we automatically annotate pre-training data by distilling annotations from a large language model into efficient classifiers. This allows us to study how data from different domains should be mixed to improve models on downstream tasks, and we show that we can combine insights about effective topics and formats to further boost performance. We demonstrate that our domain mixing also improves existing methods that select data based on quality. Furthermore, we study and compare how quality-based methods will implicitly change the domain mixture. Overall, our work demonstrates that constructing and mixing domains provides a valuable complement to quality-based data curation methods, opening new avenues for effective and insightful pre-training data curation.

웹 코퍼스를 주제와 포맷으로 분류한 다음 이 분류에 데이터 비율 결정을 위한 알고리즘을 적용해 (https://arxiv.org/abs/2407.01492) 프리트레이닝을 시도했군요.

<english>
The study on classifying web corpus by topics and formats. After it pretraining was done by applying algorithms for optimize sampling ratio of domains (https://arxiv.org/abs/2407.01492).
</english>

#corpus #pretraining 