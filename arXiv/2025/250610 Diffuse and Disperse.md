https://arxiv.org/abs/2506.09027

*Diffuse and Disperse: Image Generation with Representation Regularization* (Runqian Wang, Kaiming He)

> The development of diffusion-based generative models over the past decade has largely proceeded independently of progress in representation learning. These diffusion models typically rely on regression-based objectives and generally lack explicit regularization. In this work, we propose \textit{Dispersive Loss}, a simple plug-and-play regularizer that effectively improves diffusion-based generative models. Our loss function encourages internal representations to disperse in the hidden space, analogous to contrastive self-supervised learning, with the key distinction that it requires no positive sample pairs and therefore does not interfere with the sampling process used for regression. Compared to the recent method of representation alignment (REPA), our approach is self-contained and minimalist, requiring no pre-training, no additional parameters, and no external data. We evaluate Dispersive Loss on the ImageNet dataset across a range of models and report consistent improvements over widely used and strong baselines. We hope our work will help bridge the gap between generative modeling and representation learning.

샘플 사이의 차이를 증가시키는 Loss를 사용한 Diffusion 모델 개선. 원 Objective와는 관계 없는 Objective의 추가로 성능이 향상되는 건 늘 재미있죠.

<english>
Improving diffusion model using the loss increases difference in samples. It is always interesting when auxiliary objective in addition to original objective actually improves the performance.
</english>

#diffusion #regularization 