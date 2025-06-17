https://arxiv.org/abs/2411.14402

*Multimodal Autoregressive Pre-training of Large Vision Encoders* (Enrico Fini, Mustafa Shukor, Xiujun Li, Philipp Dufter, Michal Klein, David Haldimann, Sai Aitharaju, Victor Guilherme Turrisi da Costa, Louis Béthune, Zhe Gan, Alexander T Toshev, Marcin Eichner, Moin Nabi, Yinfei Yang, Joshua M. Susskind, Alaaeldin El-Nouby)

> We introduce a novel method for pre-training of large-scale vision encoders. Building on recent advancements in autoregressive pre-training of vision models, we extend this framework to a multimodal setting, i.e., images and text. In this paper, we present AIMV2, a family of generalist vision encoders characterized by a straightforward pre-training process, scalability, and remarkable performance across a range of downstream tasks. This is achieved by pairing the vision encoder with a multimodal decoder that autoregressively generates raw image patches and text tokens. Our encoders excel not only in multimodal evaluations but also in vision benchmarks such as localization, grounding, and classification. Notably, our AIMV2-3B encoder achieves 89.5% accuracy on ImageNet-1k with a frozen trunk. Furthermore, AIMV2 consistently outperforms state-of-the-art contrastive models (e.g., CLIP, SigLIP) in multimodal image understanding across diverse settings.

Vision-Language 모델에서 이미지 패치에는 Prefix LM Objective로 픽셀 예측을, 캡션에 대해서는 Autoregressive Loss를 사용.

Vision-Language 모델에서 텍스트는 이미지에 대해 입출력 인터페이스를 제공한다는 느낌이죠. 이미지에 대해서는 이미지에서 더 많은 정보를 끌어내기 위한 방법이 있을 것이라는 생각입니다. 다만 그 정보를 어떻게 인터페이스와 연결할 것인가는 다른 문제겠죠. (물론 모델이 커지면 이 두 모달리티를 알아서 정렬할 수도 있을 것 같긴 합니다.)

<english>
Pretraining objective for vision language models. Use prefix lm objective with pixel prediction is used for image patches, and autoregressive loss for captions.

I think text in vision language models is a kind of interface for input and output. So maybe there are a method that would extract more information from the images. But it is still a problem how we can connect that information with some interfaces. (Of course, as model became larger, maybe model can align these two modelities by itself.)
</english>

#multimodal #autoregressive-model 