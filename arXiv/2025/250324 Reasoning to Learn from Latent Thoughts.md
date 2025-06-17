https://arxiv.org/abs/2503.18866

*Reasoning to Learn from Latent Thoughts* (Yangjun Ruan, Neil Band, Chris J. Maddison, Tatsunori Hashimoto)

> Compute scaling for language model (LM) pretraining has outpaced the growth of human-written texts, leading to concerns that data will become the bottleneck to LM scaling. To continue scaling pretraining in this data-constrained regime, we propose that explicitly modeling and inferring the latent thoughts that underlie the text generation process can significantly improve pretraining data efficiency. Intuitively, our approach views web text as the compressed final outcome of a verbose human thought process and that the latent thoughts contain important contextual knowledge and reasoning steps that are critical to data-efficient learning. We empirically demonstrate the effectiveness of our approach through data-constrained continued pretraining for math. We first show that synthetic data approaches to inferring latent thoughts significantly improve data efficiency, outperforming training on the same amount of raw data (5.7\% $\rightarrow$ 25.4\% on MATH). Furthermore, we demonstrate latent thought inference without a strong teacher, where an LM bootstraps its own performance by using an EM algorithm to iteratively improve the capability of the trained LM and the quality of thought-augmented pretraining data. We show that a 1B LM can bootstrap its performance across at least three iterations and significantly outperform baselines trained on raw data, with increasing gains from additional inference compute when performing the E-step. The gains from inference scaling and EM iterations suggest new opportunities for scaling data-constrained pretraining.

일반적인 텍스트에 대해 추론 텍스트를 생성해 데이터를 확장할 수 있는가 하는 연구. 프리트레이닝 데이터의 규모의 한계를 극복하기 위한 중요한 방향이겠죠. 더 중요한 것은 모델이 주어진 데이터를 통해 데이터의 증강 과정을 Bootstrapping 할 수 있는가일 텐데 Importance Sampling을 통해 그걸 시도해봤네요.

<english>
Research on whether it is possible to extend the data by generate reasoning texts for general texts. It would be important research direction to overcome limitation of pretraining data sizes. More important problem would be whether it is possible for model to bootstrap data augmentation processes for given data by itself, and the authors tried it using importance sampling.
</english>

#synthetic-data #reasoning #pretraining 