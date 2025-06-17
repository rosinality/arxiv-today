https://arxiv.org/abs/2410.03083

*Scaling Parameter-Constrained Language Models with Quality Data* (Ernie Chang, Matteo Paltenghi, Yang Li, Pin-Jie Lin, Changsheng Zhao, Patrick Huber, Zechun Liu, Rastislav Rabatin, Yangyang Shi, Vikas Chandra)

> Scaling laws in language modeling traditionally quantify training loss as a function of dataset size and model parameters, providing compute-optimal estimates but often neglecting the impact of data quality on model generalization. In this paper, we extend the conventional understanding of scaling law by offering a microscopic view of data quality within the original formulation -- effective training tokens -- which we posit to be a critical determinant of performance for parameter-constrained language models. Specifically, we formulate the proposed term of effective training tokens to be a combination of two readily-computed indicators of text: (i) text diversity and (ii) syntheticity as measured by a teacher model. We pretrained over $200$ models of 25M to 1.5B parameters on a diverse set of sampled, synthetic data, and estimated the constants that relate text quality, model size, training tokens, and eight reasoning task accuracy scores. We demonstrated the estimated constants yield +0.83 Pearson correlation with true accuracies, and analyzed it in scenarios involving widely-used data techniques such as data sampling and synthesis which aim to improve data quality.

데이터 품질을 고려한 Scaling Law를 추정. 데이터의 품질은 Diversity = gzip 압축률의 역수, Syntheticity = Perplexity의 역수로 추정했습니다.

관계가 아주 깨끗한 것 같지는 않지만 저자들의 결론은 모델이 작다면 Syntheticity, 즉 합성 데이터가 도움이 될 수 있지만 모델이 커질수록 학습 토큰의 양 자체가 중요해진다는 것이네요.

<english>
Estimating scaling law considering data qualities. Data quality is estimated by diversity which is inverse of gzip compression rate, and syntheticity which is inverse of perplexity.

I think the relationship is not very clean, but the conclusion of the authors is that for smaller models syntheticity, which is synthetic data, could be beneficial, but for larger models absolute number of training token itself is more important.
</english>

#synthetic-data #scaling-law 