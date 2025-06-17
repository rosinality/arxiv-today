https://arxiv.org/abs/2410.15225

*Chasing Random: Instruction Selection Strategies Fail to Generalize* (Harshita Diddee, Daphne Ippolito)

> Prior work has shown that language models can be tuned to follow user instructions using only a small set of high-quality instructions. This has accelerated the development of methods that filter a large, noisy instruction-tuning datasets down to high-quality subset which works just as well. However, typically, the performance of these methods is not demonstrated across a uniform experimental setup and thus their generalization capabilities are not well established. In this work, we analyze popular selection strategies across different source datasets, selection budgets and evaluation benchmarks: Our results indicate that selection strategies generalize poorly, often failing to consistently outperform even random baselines. We also analyze the cost-performance trade-offs of using data selection. Our findings reveal that data selection can often exceed the cost of fine-tuning on the full dataset, yielding only marginal and sometimes no gains compared to tuning on the full dataset or a random subset.

Instruction 데이터 선택 방법이 다양한 과제나 데이터셋에 대해 랜덤 선택보다도 (특히 비용까지 고려한다면) 안정적으로 더 나은 결과를 얻기 어렵다는 분석. 비슷한 결과가 얼마 전에도 나왔었죠. (https://arxiv.org/abs/2410.09335) 복잡하고 정교한 방법이 랜덤보다 확연히 우수하지 않은 것도 전형적인 패턴이긴 합니다.

<english>
Analysis that it is hard for sophisticated data selection methods to beat random sampling reliably on instruction samplings. Similar results came out some day ago. (https://arxiv.org/abs/2410.09335) It is common pattern that sophisticated and complex method fail to surpass mere random methods.
</english>

#alignment #dataset

# Links

[[241012 Rethinking Data Selection at Scale.md]]