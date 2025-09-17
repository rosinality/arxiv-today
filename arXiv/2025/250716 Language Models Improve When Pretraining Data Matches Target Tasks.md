https://arxiv.org/abs/2507.12466

*Language Models Improve When Pretraining Data Matches Target Tasks* (David Mizrahi, Anders Boesen Lindbo Larsen, Jesse Allardice, Suzie Petryk, Yuri Gorokhov, Jeffrey Li, Alex Fang, Josh Gardner, Tom Gunter, Afshin Dehghan)

> Every data selection method inherently has a target. In practice, these targets often emerge implicitly through benchmark-driven iteration: researchers develop selection strategies, train models, measure benchmark performance, then refine accordingly. This raises a natural question: what happens when we make this optimization explicit? To explore this, we propose benchmark-targeted ranking (BETR), a simple method that selects pretraining documents based on similarity to benchmark training examples. BETR embeds benchmark examples and a sample of pretraining documents in a shared space, scores this sample by similarity to benchmarks, then trains a lightweight classifier to predict these scores for the full corpus. We compare data selection methods by training over 500 models spanning $10^{19}$ to $10^{22}$ FLOPs and fitting scaling laws to them. From this, we find that simply aligning pretraining data to evaluation benchmarks using BETR achieves a 2.1x compute multiplier over DCLM-Baseline (4.7x over unfiltered data) and improves performance on 9 out of 10 tasks across all scales. BETR also generalizes well: when targeting a diverse set of benchmarks disjoint from our evaluation suite, it still matches or outperforms baselines. Our scaling analysis further reveals a clear trend: larger models require less aggressive filtering. Overall, our findings show that directly matching pretraining data to target tasks precisely shapes model capabilities and highlight that optimal selection strategies must adapt to model scale.

벤치마크와 유사한 텍스트를 찾는 방법으로 프리트레이닝 데이터 필터링하기. 단순한 벤치마크 해킹은 아니고 훨씬 미묘합니다. 보통 인기 있는 벤치마크로 필터링하면 해킹이 일어난다는 것, 더 다양한 벤치마크를 사용하면 경쟁력이 있는 것 같다는 걸 보고하고 있군요. 벤치마크를 타겟한 데이터 필터링이 흔하다는 걸 고려하면 그걸 지나치게 추구했을 때 어떤 위험이 있는지를 보여주는 것이겠죠.

모델 규모가 커질수록 필터링을 약하게 하는 쪽이 낫다는 분석도 있습니다. 모델 크기가 작으면 이 경향이 작다고 하는군요. 큰 모델과 작은 모델의 차이가 이런 지점에서도 나타날 수 있겠죠.

<english>
Filtering pretraining data by find out similar texts with benchmarks. It is more delicate beyond just benchmark hacking. It shows that hacking occurs when we only use popular benchmarks for filtering, though it could be competitive against to other filtering methods if we use diverse benchmarks. It could shows that the risk when we pursues too much on targeting benchmarks, considering it is common to filter datasets for these benchmark scores.

There is also analysis that lighter filtering could be better when model sizes became larger. This trend is weaker for smaller models. Maybe this could be also point that causes difference between larger and smaller models.
</english>

#pretraining #scaling-law #corpus 