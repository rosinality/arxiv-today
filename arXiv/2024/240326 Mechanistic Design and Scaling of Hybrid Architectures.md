https://arxiv.org/abs/2403.17844

*Mechanistic Design and Scaling of Hybrid Architectures* (Michael Poli, Armin W Thomas, Eric Nguyen, Pragaash Ponnusamy, Björn Deiseroth, Kristian Kersting, Taiji Suzuki, Brian Hie, Stefano Ermon, Christopher Ré, Ce Zhang, Stefano Massaroli)

> The development of deep learning architectures is a resource-demanding process, due to a vast design space, long prototyping times, and high compute costs associated with at-scale model training and evaluation. We set out to simplify this process by grounding it in an end-to-end mechanistic architecture design (MAD) pipeline, encompassing small-scale capability unit tests predictive of scaling laws. Through a suite of synthetic token manipulation tasks such as compression and recall, designed to probe capabilities, we identify and test new hybrid architectures constructed from a variety of computational primitives. We experimentally validate the resulting architectures via an extensive compute-optimal and a new state-optimal scaling law analysis, training over 500 language models between 70M to 7B parameters. Surprisingly, we find MAD synthetics to correlate with compute-optimal perplexity, enabling accurate evaluation of new architectures via isolated proxy tasks. The new architectures found via MAD, based on simple ideas such as hybridization and sparsity, outperform state-of-the-art Transformer, convolutional, and recurrent architectures (Transformer++, Hyena, Mamba) in scaling, both at compute-optimal budgets and in overtrained regimes. Overall, these results provide evidence that performance on curated synthetic tasks can be predictive of scaling laws, and that an optimal architecture should leverage specialized layers via a hybrid topology.

State Space Model과 Transformer의 하이브리드 모델들에 대한 Scaling Law. Attention을 25% 정도 섞은 모델이 최적이었다고 합니다. 더 나아가 하이브리드 모델이 더 작은 모델을 더 오래 학습하는 측면에서 유리했다고 하네요.

Associative Recall 같은 과제가 시퀀스 모델의 특성에 대해 알려주는 것이 많죠. 이런 Synthetic한 토큰 조작 과제들이 Scaling Law와 어떻게 연결될 수 있는지를 테스트했습니다. 토큰 조작 과제들에 대한 성능과 Compute Optimal 모델의 Perplexity 사이에 선형적인 관계가 나타났네요. 즉 작은 규모의 Synthetic 과제에 대한 성능으로 효과적인 아키텍처를 찾을 수도 있다는 의미가 될 수 있습니다.

하이브리드 아키텍처는 Transformer의 이후 모델로서 꽤 유망하지 않은가 싶습니다. 더 효율적이라는 것 외에도 State Space Model이 모델의 특성에 줄 수 있는 바람직한 특징이 있지 않을까 하는 생각을 합니다.

#scaling-law #transformer #state-space-model 