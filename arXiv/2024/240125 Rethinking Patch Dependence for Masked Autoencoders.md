https://arxiv.org/abs/2401.14391

*Rethinking Patch Dependence for Masked Autoencoders* (Letian Fu, Long Lian, Renhao Wang, Baifeng Shi, Xudong Wang, Adam Yala, Trevor Darrell, Alexei A. Efros, Ken Goldberg)

> In this work, we re-examine inter-patch dependencies in the decoding mechanism of masked autoencoders (MAE). We decompose this decoding mechanism for masked patch reconstruction in MAE into self-attention and cross-attention. Our investigations suggest that self-attention between mask patches is not essential for learning good representations. To this end, we propose a novel pretraining framework: Cross-Attention Masked Autoencoders (CrossMAE). CrossMAE's decoder leverages only cross-attention between masked and visible tokens, with no degradation in downstream performance. This design also enables decoding only a small subset of mask tokens, boosting efficiency. Furthermore, each decoder block can now leverage different encoder features, resulting in improved representation learning. CrossMAE matches MAE in performance with 2.5 to 3.7$\times$ less decoding compute. It also surpasses MAE on ImageNet classification and COCO instance segmentation under the same compute. Code and models: https://crossmae.github.io

Masked Autoencoder에서 디코더를 이미지 패치와 마스크 토큰을 입력으로 받는 트랜스포머로 설정하는 대신 마스크 토큰과 이미지 패치 사이의 Cross Attention으로 바꾸고 Self Attention을 아예 빼버렸습니다. 따라서 마스크 토큰들은 서로 독립이 되고 그래서 일부만 디코딩하는 것도 가능해집니다. 추가로 여러 단계의 Feature를 선형 결합하는 디자인도 고려했네요.

전반적으로 성능을 동등하게 유지하면서 효율성을 높인다는 형태의 결과이긴 합니다. 제안하는 것처럼 비디오 같은 대상에 대해서 고려가 가능하겠네요.

#self-supervision #mlm 