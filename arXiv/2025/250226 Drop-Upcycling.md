https://arxiv.org/abs/2502.19261

*Drop-Upcycling: Training Sparse Mixture of Experts with Partial Re-initialization* (Taishi Nakamura, Takuya Akiba, Kazuki Fujii, Yusuke Oda, Rio Yokota, Jun Suzuki)

> The Mixture of Experts (MoE) architecture reduces the training and inference cost significantly compared to a dense model of equivalent capacity. Upcycling is an approach that initializes and trains an MoE model using a pre-trained dense model. While upcycling leads to initial performance gains, the training progresses slower than when trained from scratch, leading to suboptimal performance in the long term. We propose Drop-Upcycling - a method that effectively addresses this problem. Drop-Upcycling combines two seemingly contradictory approaches: utilizing the knowledge of pre-trained dense models while statistically re-initializing some parts of the weights. This approach strategically promotes expert specialization, significantly enhancing the MoE model's efficiency in knowledge acquisition. Extensive large-scale experiments demonstrate that Drop-Upcycling significantly outperforms previous MoE construction methods in the long term, specifically when training on hundreds of billions of tokens or more. As a result, our MoE model with 5.9B active parameters achieves comparable performance to a 13B dense model in the same model family, while requiring approximately 1/4 of the training FLOPs. All experimental resources, including source code, training data, model checkpoints and logs, are publicly available to promote reproducibility and future research on MoE.

Sparse Upcycling에서 FFN을 그대로 복제하는 대신 Perturbation을 줘서 다양성을 높인 방법. From Scratch 학습에 비교해서 성능 향상이 감소한다는 결과에서 생각할 수 있는 방향이죠. 물론 성능 역전이 발생하는 지점을 옮기는 정도일 수도 있겠습니다만.

<english>
A method for sparse upcycling that diversifies experts by using perturbations instead of directly replicate it. It is one way to do when we found upcycling has diminishing returns compared to from scratch training. Of course it could be just moving point of loss crosses.
</english>

#moe 