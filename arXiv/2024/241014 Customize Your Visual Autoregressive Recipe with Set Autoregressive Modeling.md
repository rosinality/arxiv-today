https://arxiv.org/abs/2410.10511

*Customize Your Visual Autoregressive Recipe with Set Autoregressive Modeling* (Wenze Liu, Le Zhuo, Yi Xin, Sheng Xia, Peng Gao, Xiangyu Yue)

> We introduce a new paradigm for AutoRegressive (AR) image generation, termed Set AutoRegressive Modeling (SAR). SAR generalizes the conventional AR to the next-set setting, i.e., splitting the sequence into arbitrary sets containing multiple tokens, rather than outputting each token in a fixed raster order. To accommodate SAR, we develop a straightforward architecture termed Fully Masked Transformer. We reveal that existing AR variants correspond to specific design choices of sequence order and output intervals within the SAR framework, with AR and Masked AR (MAR) as two extreme instances. Notably, SAR facilitates a seamless transition from AR to MAR, where intermediate states allow for training a causal model that benefits from both few-step inference and KV cache acceleration, thus leveraging the advantages of both AR and MAR. On the ImageNet benchmark, we carefully explore the properties of SAR by analyzing the impact of sequence order and output intervals on performance, as well as the generalization ability regarding inference order and steps. We further validate the potential of SAR by training a 900M text-to-image model capable of synthesizing photo-realistic images with any resolution. We hope our work may inspire more exploration and application of AR-based modeling across diverse modalities.

이미지 토큰 시퀀스의 특정 집합들을 예측하는 형태로 Autoregressive 생성을 일반화. 구현은 인코더-디코더를 사용해서 했습니다. Autoregressive 생성으로도 좋은 퀄리티를 낼 수 있는가? 이 질문에 대한 다음 질문은 실용적으로 생성 속도가 충분한가가 되긴 하겠죠.

<english>
Generalizing autoregressive generation by predicting specific sets in image token sequences. Implemented using encoder-decoder. Next question after the question about whether it is possible to reach good quality using autoregressive generation, will be generation speed is within practical range.
</english>

#autoregressive-model #image-generation 