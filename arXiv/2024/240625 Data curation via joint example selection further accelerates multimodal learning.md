https://arxiv.org/abs/2406.17711

*Data curation via joint example selection further accelerates multimodal learning* (Talfan Evans, Nikhil Parthasarathy, Hamza Merzic, Olivier J. Henaff)

> Data curation is an essential component of large-scale pretraining. In this work, we demonstrate that jointly selecting batches of data is more effective for learning than selecting examples independently. Multimodal contrastive objectives expose the dependencies between data and thus naturally yield criteria for measuring the joint learnability of a batch. We derive a simple and tractable algorithm for selecting such batches, which significantly accelerate training beyond individually-prioritized data points. As performance improves by selecting from larger super-batches, we also leverage recent advances in model approximation to reduce the associated computational overhead. As a result, our approach--multimodal contrastive learning with joint example selection (JEST)--surpasses state-of-the-art models with up to 13$\times$ fewer iterations and 10$\times$ less computation. Essential to the performance of JEST is the ability to steer the data selection process towards the distribution of smaller, well-curated datasets via pretrained reference models, exposing the level of data curation as a new dimension for neural scaling laws.

CLIP에서 배치를 구성하는 방법. Hard Negative와 같이 좋은 샘플들로 배치를 구성하는 것을 목표로 합니다.

배치 구성을 위한 퀄리티의 지표는 학습 중인 모델의 Loss와 레퍼런스 모델의 Loss 차이입니다. (Learnability) 레퍼런스 모델은 고품질 데이터셋에 학습시킨 모델이죠. 최근 Rho-1 (https://arxiv.org/abs/2404.07965) 에서도 등장한 방법입니다. CLIP이기 때문에 개별 샘플을 고르는 것보다 배치를 잘 구성하는 것이 중요하고 따라서 Joint Learnability에 따라 샘플링하는 알고리즘을 설계했습니다.

흥미롭네요. 생각해 볼 만한 방법인 것 같습니다. 이 방법의 기원을 한 번 체크해보는 것도 좋을 듯 합니다. (https://arxiv.org/abs/2206.07137)

#clip 