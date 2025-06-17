https://arxiv.org/abs/2401.10208

*MM-Interleaved: Interleaved Image-Text Generative Modeling via Multi-modal Feature Synchronizer* (Changyao Tian, Xizhou Zhu, Yuwen Xiong, Weiyun Wang, Zhe Chen, Wenhai Wang, Yuntao Chen, Lewei Lu, Tong Lu, Jie Zhou, Hongsheng Li, Yu Qiao, Jifeng Dai)

> Developing generative models for interleaved image-text data has both research and practical value. It requires models to understand the interleaved sequences and subsequently generate images and text. However, existing attempts are limited by the issue that the fixed number of visual tokens cannot efficiently capture image details, which is particularly problematic in the multi-image scenarios. To address this, this paper presents MM-Interleaved, an end-to-end generative model for interleaved image-text data. It introduces a multi-scale and multi-image feature synchronizer module, allowing direct access to fine-grained image features in the previous context during the generation process. MM-Interleaved is end-to-end pre-trained on both paired and interleaved image-text corpora. It is further enhanced through a supervised fine-tuning phase, wherein the model improves its ability to follow complex multi-modal instructions. Experiments demonstrate the versatility of MM-Interleaved in recognizing visual details following multi-modal instructions and generating consistent images following both textual and visual conditions. Code and models are available at \url{https://github.com/OpenGVLab/MM-Interleaved}.

Interleaved Vision-Language 모델 + 이미지 생성. Resampler를 사용하면서 발생하는 정보 손실에 대해 Multiscale Feature를 사용해서 커버하는 방식입니다. Multiscale Feature에 대한 결합은 Deformable Attention을 사용했네요. 생각해보면 Deformable Attention은 기본적으로 Multiscale Cross Attention을 효율적으로 위해서 나온 방법이기도 하죠. 비전 하던 사람들이 붙으니 과거의 비전 쪽 접근들의 향취가 나는군요.

더해서 구글이 요즘 모델을 결합할 때 중간 레이어들을 연결하는 방법을 쓰고 있는데 (https://arxiv.org/abs/2401.02412, https://arxiv.org/abs/2401.08525) 관련지어 생각해볼 수 있지 않을까 싶네요.

#vision-language

# Links

[[240104 LLM Augmented LLMs.md]]
[[240116 GATS.md]]