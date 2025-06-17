https://arxiv.org/abs/2402.18153

*Diffusion-based Neural Network Weights Generation* (Bedionita Soro, Bruno Andreis, Hayeon Lee, Song Chong, Frank Hutter, Sung Ju Hwang)

> Transfer learning is a topic of significant interest in recent deep learning research because it enables faster convergence and improved performance on new tasks. While the performance of transfer learning depends on the similarity of the source data to the target data, it is costly to train a model on a large number of datasets. Therefore, pretrained models are generally blindly selected with the hope that they will achieve good performance on the given task. To tackle such suboptimality of the pretrained models, we propose an efficient and adaptive transfer learning scheme through dataset-conditioned pretrained weights sampling. Specifically, we use a latent diffusion model with a variational autoencoder that can reconstruct the neural network weights, to learn the distribution of a set of pretrained weights conditioned on each dataset for transfer learning on unseen datasets. By learning the distribution of a neural network on a variety pretrained models, our approach enables adaptive sampling weights for unseen datasets achieving faster convergence and reaching competitive performance.

Neural Network Diffusion (https://arxiv.org/abs/2402.13144) 같은 시나리오가 하나 더 나왔군요. 이쪽은 데이터셋에 대한 임베딩을 결합해서 데이터셋에 대한 모델을 생성하도록 했습니다.

모델을 생성하는 모델을 생성하는 모델도 가능할까요? 궁금해지네요.

#diffusion #hypernetwork

# Links

[[240220 Neural Network Diffusion.md]]