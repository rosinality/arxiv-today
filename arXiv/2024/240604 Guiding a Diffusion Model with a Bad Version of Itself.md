https://arxiv.org/abs/2406.02507

*Guiding a Diffusion Model with a Bad Version of Itself* (Tero Karras, Miika Aittala, Tuomas Kynkäänniemi, Jaakko Lehtinen, Timo Aila, Samuli Laine)

> The primary axes of interest in image-generating diffusion models are image quality, the amount of variation in the results, and how well the results align with a given condition, e.g., a class label or a text prompt. The popular classifier-free guidance approach uses an unconditional model to guide a conditional model, leading to simultaneously better prompt alignment and higher-quality images at the cost of reduced variation. These effects seem inherently entangled, and thus hard to control. We make the surprising observation that it is possible to obtain disentangled control over image quality without compromising the amount of variation by guiding generation using a smaller, less-trained version of the model itself rather than an unconditional model. This leads to significant improvements in ImageNet generation, setting record FIDs of 1.01 for 64x64 and 1.25 for 512x512, using publicly available networks. Furthermore, the method is also applicable to unconditional diffusion models, drastically improving their quality.

Karras 선생님이 한 건 더 하셨군요. Classifier-free Guidance가 퀄리티와 프롬프트에 대한 정렬을 높이면서 다양성을 감소시키는데, Guidance를 위한 모델로 Unconditional 모델이 아니라 Condition이 주어진 동일한 모델, 그렇지만 좀 더 약한 모델, 즉 더 작고 학습이 덜 된 모델을 사용하는 것으로 퀄리티를 높이면서 다양성의 감소도 억제할 수 있다는 결과입니다.

#diffusion 