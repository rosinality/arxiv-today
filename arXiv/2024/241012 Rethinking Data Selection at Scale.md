https://arxiv.org/abs/2410.09335

*Rethinking Data Selection at Scale: Random Selection is Almost All You Need* (Tingyu Xia, Bowen Yu, Kai Dang, An Yang, Yuan Wu, Yuan Tian, Yi Chang, Junyang Lin)

> Supervised fine-tuning (SFT) is crucial for aligning Large Language Models (LLMs) with human instructions. The primary goal during SFT is to select a small yet representative subset of training data from the larger pool, such that fine-tuning with this subset achieves results comparable to or even exceeding those obtained using the entire dataset. However, most existing data selection techniques are designed for small-scale data pools, which fail to meet the demands of real-world SFT scenarios. In this paper, we replicated several self-scoring methods those that do not rely on external model assistance on two million scale datasets, and found that nearly all methods struggled to significantly outperform random selection when dealing with such large-scale data pools. Moreover, our comparisons suggest that, during SFT, diversity in data selection is more critical than simply focusing on high quality data. We also analyzed the limitations of several current approaches, explaining why they perform poorly on large-scale datasets and why they are unsuitable for such contexts. Finally, we found that filtering data by token length offers a stable and efficient method for improving results. This approach, particularly when training on long text data, proves highly beneficial for relatively weaker base models, such as Llama3.

SFT 데이터셋 샘플링 문제에서 데이터셋 규모가 증가했을 때 랜덤 선택이 다른 방법을 사용한 것보다 나았다는 결과.

<english>
For SFT dataset sampling problems, plain random sampling was better than the other methods when dataset size is increased.
</english>

#alignment #dataset 