https://arxiv.org/abs/2405.10939

*DINO as a von Mises-Fisher mixture model* (Hariprasath Govindarajan, Per Sidén, Jacob Roll, Fredrik Lindsten)

> Self-distillation methods using Siamese networks are popular for self-supervised pre-training. DINO is one such method based on a cross-entropy loss between $K$-dimensional probability vectors, obtained by applying a softmax function to the dot product between representations and learnt prototypes. Given the fact that the learned representations are $L^2$-normalized, we show that DINO and its derivatives, such as iBOT, can be interpreted as a mixture model of von Mises-Fisher components. With this interpretation, DINO assumes equal precision for all components when the prototypes are also $L^2$-normalized. Using this insight we propose DINO-vMF, that adds appropriate normalization constants when computing the cluster assignment probabilities. Unlike DINO, DINO-vMF is stable also for the larger ViT-Base model with unnormalized prototypes. We show that the added flexibility of the mixture model is beneficial in terms of better image representations. The DINO-vMF pre-trained model consistently performs better than DINO on a range of downstream tasks. We obtain similar improvements for iBOT-vMF vs iBOT and thereby show the relevance of our proposed modification also for other methods derived from DINO.

DINO의 학습 Objective를 vMF 분포 Mixture 모델로 연결해봤을 때 vMF Mixture에 있어야 할 Normalization constant가 빠져 있는데 이 상수의 부재가 학습 불안정성을 유발한다는 아이디어. 재미있네요.

#contrastive-learning 