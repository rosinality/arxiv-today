https://arxiv.org/abs/2503.05305

*Frequency Autoregressive Image Generation with Continuous Tokens* (Hu Yu, Hao Luo, Hangjie Yuan, Yu Rong, Feng Zhao)

> Autoregressive (AR) models for image generation typically adopt a two-stage paradigm of vector quantization and raster-scan ``next-token prediction", inspired by its great success in language modeling. However, due to the huge modality gap, image autoregressive models may require a systematic reevaluation from two perspectives: tokenizer format and regression direction. In this paper, we introduce the frequency progressive autoregressive (\textbf{FAR}) paradigm and instantiate FAR with the continuous tokenizer. Specifically, we identify spectral dependency as the desirable regression direction for FAR, wherein higher-frequency components build upon the lower one to progressively construct a complete image. This design seamlessly fits the causality requirement for autoregressive models and preserves the unique spatial locality of image data. Besides, we delve into the integration of FAR and the continuous tokenizer, introducing a series of techniques to address optimization challenges and improve the efficiency of training and inference processes. We demonstrate the efficacy of FAR through comprehensive experiments on the ImageNet dataset and verify its potential on text-to-image generation.

주파수 영역에서의 Autoregressive Image Generation. Loss로는 MAR 스타일의 Diffusion Loss를 사용했습니다. VAR에서는 Continuous Token을 사용하는 것이 잘 안 됐다고 하는군요. 그 부분을 개선하려는 것이 주된 문제 의식이었던 것 같습니다. (성능과는 별개로.)

<english>
Autoregressive image generation on frequency domain. They used MAR (https://arxiv.org/abs/2406.11838) style diffusion loss. They mention that VAR (https://arxiv.org/abs/2404.02905) does not work very well on continuous tokens. Maybe the main point of this resarch is to resolve that problem. (Regardless performances.)
</english>

#autoregressive-model #diffusion 