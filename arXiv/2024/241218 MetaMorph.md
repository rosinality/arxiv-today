https://arxiv.org/abs/2412.14164

*MetaMorph: Multimodal Understanding and Generation via Instruction Tuning* (Shengbang Tong, David Fan, Jiachen Zhu, Yunyang Xiong, Xinlei Chen, Koustuv Sinha, Michael Rabbat, Yann LeCun, Saining Xie, Zhuang Liu)

> In this work, we propose Visual-Predictive Instruction Tuning (VPiT) - a simple and effective extension to visual instruction tuning that enables a pretrained LLM to quickly morph into an unified autoregressive model capable of generating both text and visual tokens. VPiT teaches an LLM to predict discrete text tokens and continuous visual tokens from any input sequence of image and text data curated in an instruction-following format. Our empirical investigation reveals several intriguing properties of VPiT: (1) visual generation ability emerges as a natural byproduct of improved visual understanding, and can be unlocked efficiently with a small amount of generation data; (2) while we find understanding and generation to be mutually beneficial, understanding data contributes to both capabilities more effectively than generation data. Building upon these findings, we train our MetaMorph model and achieve competitive performance on both visual understanding and generation. In visual generation, MetaMorph can leverage the world knowledge and reasoning abilities gained from LLM pretraining, and overcome common failure modes exhibited by other generation models. Our results suggest that LLMs may have strong "prior" vision capabilities that can be efficiently adapted to both visual understanding and generation with a relatively simple instruction tuning process.

이미지 Feature를 예측하는 단순한 Objective로 이미지 생성 능력을 탑재한 다음 이미지 인식과 이미지 생성 과제 데이터로 학습했을 때의 결과 분석. 이미지 생성과 인식이 서로에게 도움이 되고 (인식이 좀 더 도움이 되긴 하지만) 이미지 생성 데이터가 지식과 구분된 이미지 자체의 인식 능력에 도움이 될 수 있다는 결과네요.

<english>
Adding image generation capability using simple objective that predicts image feature, and analyze the result of training using image recognition and generation task data. Image recognition and generation is beneficial for each other (though recognition has more gain) and image generation data could be more useful for image recognition capability itself separated from knowledge.
</english>

#autoregressive-model #text-to-image #vision-language 