https://arxiv.org/abs/2404.08636

*Probing the 3D Awareness of Visual Foundation Models* (Mohamed El Banani, Amit Raj, Kevis-Kokitsi Maninis, Abhishek Kar, Yuanzhen Li, Michael Rubinstein, Deqing Sun, Leonidas Guibas, Justin Johnson, Varun Jampani)

> Recent advances in large-scale pretraining have yielded visual foundation models with strong capabilities. Not only can recent models generalize to arbitrary images for their training task, their intermediate representations are useful for other visual tasks such as detection and segmentation. Given that such models can classify, delineate, and localize objects in 2D, we ask whether they also represent their 3D structure? In this work, we analyze the 3D awareness of visual foundation models. We posit that 3D awareness implies that representations (1) encode the 3D structure of the scene and (2) consistently represent the surface across views. We conduct a series of experiments using task-specific probes and zero-shot inference procedures on frozen features. Our experiments reveal several limitations of the current models. Our code and analysis can be found at https://github.com/mbanani/probe3d.

Depth/Surface Normal/Correspondence Estimation으로 CLIP, DINO, StableDiffusion 같은 Vision 인코더 모델들의 3d Awareness를 측정했군요.

DINO와 Stable Diffusion이 꽤 좋은 성능을 보여줍니다. 다만 Correspondence에서 모델들이 모두 약한 모습을 보여주네요. 3D Consistency에 대해 문제가 있다는 의미가 됩니다.

비디오나 3D 데이터에 대해 Contrastive 혹은 Generative Objective로 학습된 인코더가 가장 우수한 특성을 보여줄 것 같다는 느낌이 드네요.

#vision 