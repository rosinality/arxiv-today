https://arxiv.org/abs/2402.03161

*Video-LaVIT: Unified Video-Language Pre-training with Decoupled Visual-Motional Tokenization* (Yang Jin, Zhicheng Sun, Kun Xu, Kun Xu, Liwei Chen, Hao Jiang, Quzhe Huang, Chengru Song, Yuliang Liu, Di Zhang, Yang Song, Kun Gai, Yadong Mu)

> In light of recent advances in multimodal Large Language Models (LLMs), there is increasing attention to scaling them from image-text data to more informative real-world videos. Compared to static images, video poses unique challenges for effective large-scale pre-training due to the modeling of its spatiotemporal dynamics. In this paper, we address such limitations in video-language pre-training with an efficient video decomposition that represents each video as keyframes and temporal motions. These are then adapted to an LLM using well-designed tokenizers that discretize visual and temporal information as a few tokens, thus enabling unified generative pre-training of videos, images, and text. At inference, the generated tokens from the LLM are carefully recovered to the original continuous pixel space to create various video content. Our proposed framework is both capable of comprehending and generating image and video content, as demonstrated by its competitive performance across 13 multimodal benchmarks in image and video understanding and generation. Our code and models will be available at https://video-lavit.github.io.

https://video-lavit.github.io/

Video-Text에 대한 Autoregressive 모델링. 영상을 키프레임과 모션으로 분해하고, 이 둘을 모두 Quantization해서 텍스트와 함께 Autoregressive 학습을 시킵니다. 이 위에 Detokenizer를 올려 비디오와 텍스트에 대한 생성이 가능하게 했네요. 비디오에 대한 흥미로운 접근이 아닌가 싶습니다.

#video-generation #video-text #multimodal 

Autoregressive modeling for video-text. First decompose video into keyframes and motions, then quantize both of it and do autoregressive training with the text. On the top of that detokenizer is used to make it generate both video and text. I think this is interesting approach for video modeling.