https://arxiv.org/abs/2311.05698

Mirasol3B: A Multimodal Autoregressive model for time-aligned and contextual modalities (AJ Piergiovanni, Isaac Noble, Dahun Kim, Michael S. Ryoo, Victor Gomes, Anelia Angelova)

비디오, 오디오, 텍스트에 대한 multimodal 모델. 비디오와 오디오는 서로 정렬되어 있다고 보고, ViT로 임베딩한 다음 Combiner로 결합합니다. Combiner로는 트랜스포머나 토큰 튜링 머신(!)을 사용합니다. 이렇게 결합된 임베딩을 autoregressive latent 트랜스포머에 입력하고, 이 latent 임베딩을 autoregressive reconstruction 트랜스포머에 넣어 비디오와 오디오를 예측하게 합니다. 이 모델에서 나온 latent 임베딩을 텍스트 디코더와 cross attetnion으로 결합했네요. 대체 트랜스포머가 몇 종류 사용된 걸까요.

#video #multimodal 