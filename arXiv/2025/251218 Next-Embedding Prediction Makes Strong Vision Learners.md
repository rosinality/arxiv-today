https://arxiv.org/abs/2512.16922

*Next-Embedding Prediction Makes Strong Vision Learners* (Sihan Xu, Ziqiao Ma, Wenhao Chai, Xuweiyi Chen, Weiyang Jin, Joyce Chai, Saining Xie, Stella X. Yu)

> Inspired by the success of generative pretraining in natural language, we ask whether the same principles can yield strong self-supervised visual learners. Instead of training models to output features for downstream use, we train them to generate embeddings to perform predictive tasks directly. This work explores such a shift from learning representations to learning models. Specifically, models learn to predict future patch embeddings conditioned on past ones, using causal masking and stop gradient, which we refer to as Next-Embedding Predictive Autoregression (NEPA). We demonstrate that a simple Transformer pretrained on ImageNet-1k with next embedding prediction as its sole learning objective is effective - no pixel reconstruction, discrete tokens, contrastive loss, or task-specific heads. This formulation retains architectural simplicity and scalability, without requiring additional design complexity. NEPA achieves strong results across tasks, attaining 83.8% and 85.3% top-1 accuracy on ImageNet-1K with ViT-B and ViT-L backbones after fine-tuning, and transferring effectively to semantic segmentation on ADE20K. We believe generative pretraining from embeddings provides a simple, scalable, and potentially modality-agnostic alternative to visual self-supervised learning.

다음 스텝 임베딩 예측을 사용한 간단한 이미지 프리트레이닝. 임베딩 자체도 같이 학습됨. 다만 Loss 타겟으로 사용할 때에는 Stop Grad를 적용.

Simple vision pretraining by predicting next step embedding. The embedding itself is trained along with this while stop grad is applied when it is used as a target.

#pretraining #self-supervision 