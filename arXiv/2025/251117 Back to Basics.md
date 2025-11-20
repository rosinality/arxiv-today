https://arxiv.org/abs/2511.13720

*Back to Basics: Let Denoising Generative Models Denoise* (Tianhong Li, Kaiming He)

> Today's denoising diffusion models do not "denoise" in the classical sense, i.e., they do not directly predict clean images. Rather, the neural networks predict noise or a noised quantity. In this paper, we suggest that predicting clean data and predicting noised quantities are fundamentally different. According to the manifold assumption, natural data should lie on a low-dimensional manifold, whereas noised quantities do not. With this assumption, we advocate for models that directly predict clean data, which allows apparently under-capacity networks to operate effectively in very high-dimensional spaces. We show that simple, large-patch Transformers on pixels can be strong generative models: using no tokenizer, no pre-training, and no extra loss. Our approach is conceptually nothing more than "$\textbf{Just image Transformers}$", or $\textbf{JiT}$, as we call it. We report competitive results using JiT with large patch sizes of 16 and 32 on ImageNet at resolutions of 256 and 512, where predicting high-dimensional noised quantities can fail catastrophically. With our networks mapping back to the basics of the manifold, our research goes back to basics and pursues a self-contained paradigm for Transformer-based diffusion on raw natural data.

다시 한 번 차원 문제로. x가 노이즈에 비해 훨씬 낮은 차원을 갖기 때문에 고차원의 입력에 대해서는 x 예측이 ε 혹은 v 예측에 비해 훨씬 잘 작동함. x 예측은 패치 크기 64의 픽셀 입력에 대해서도 작동함!

Dimension problem again. As x has much lower dimension compared to noise, x-prediction works better compared to ε or v prediction for large dimensional inputs. x-prediction even works on pixels with patch size 64!

#diffusion #tokenizer 