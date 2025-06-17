https://arxiv.org/abs/2412.04431

*Infinity: Scaling Bitwise AutoRegressive Modeling for High-Resolution Image Synthesis* (Jian Han, Jinlai Liu, Yi Jiang, Bin Yan, Yuqi Zhang, Zehuan Yuan, Bingyue Peng, Xiaobing Liu)

> We present Infinity, a Bitwise Visual AutoRegressive Modeling capable of generating high-resolution, photorealistic images following language instruction. Infinity redefines visual autoregressive model under a bitwise token prediction framework with an infinite-vocabulary tokenizer & classifier and bitwise self-correction mechanism, remarkably improving the generation capacity and details. By theoretically scaling the tokenizer vocabulary size to infinity and concurrently scaling the transformer size, our method significantly unleashes powerful scaling capabilities compared to vanilla VAR. Infinity sets a new record for autoregressive text-to-image models, outperforming top-tier diffusion models like SD3-Medium and SDXL. Notably, Infinity surpasses SD3-Medium by improving the GenEval benchmark score from 0.62 to 0.73 and the ImageReward benchmark score from 0.87 to 0.96, achieving a win rate of 66%. Without extra optimization, Infinity generates a high-quality 1024x1024 image in 0.8 seconds, making it 2.6x faster than SD3-Medium and establishing it as the fastest text-to-image model. Models and codes will be released to promote further exploration of Infinity for visual generation and unified tokenizer modeling.

VAR (https://arxiv.org/abs/2404.02905) 기반의 Autoregression, Residual BSQ (https://arxiv.org/abs/2406.07548) 기반으로 Quantization. 그러나 정수 인덱스를 예측하는 대신 각 비트를 예측하는 방법으로 바꿔 2^32에 달하는 Vocabulary를 지원할 수 있게 했네요. 추가적으로 Autoregression 과정의 오류 누적을 비트를 뒤집은 코드를 학습에 사용해 보정할 수 있도록 했습니다. 굉장히 흥미롭네요. 비트에 대한 Autoregressive 생성만 잘 작동한다면 VQ에서는 문제가 거의 해소될 수 있지 않을까 싶습니다.

<english>
Autoregression based on VAR (https://arxiv.org/abs/2404.02905) and quantization based on residual BSQ (https://arxiv.org/abs/2406.07548). But instead of predicting integer index, the authors have adopted to predict individual bits (multi-label classification). Additionally they dealt with error accumulation on autoregressive predictions by using with bit-flipped inputs. Very intriguing. If we can make autoregressive genration on bits works well then we can resolve most issues originates from VQ.
</english>

#vq #autoregressive-model

# Links

[[240611 Image and Video Tokenization with Binary Spherical Quantization.md]]
[[240403 Visual Autoregressive Modeling.md]]