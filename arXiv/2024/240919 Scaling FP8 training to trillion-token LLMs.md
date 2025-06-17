https://arxiv.org/abs/2409.12517

*Scaling FP8 training to trillion-token LLMs* (Maxim Fishman, Brian Chmiel, Ron Banner, Daniel Soudry)

> We train, for the first time, large language models using FP8 precision on datasets up to 2 trillion tokens -- a 20-fold increase over previous limits. Through these extended training runs, we uncover critical instabilities in FP8 training that were not observable in earlier works with shorter durations. We trace these instabilities to outlier amplification by the SwiGLU activation function. Interestingly, we show, both analytically and empirically, that this amplification happens only over prolonged training periods, and link it to a SwiGLU weight alignment process. To address this newly identified issue, we introduce Smooth-SwiGLU, a novel modification that ensures stable FP8 training without altering function behavior. We also demonstrate, for the first time, FP8 quantization of both Adam optimizer moments. Combining these innovations, we successfully train a 7B parameter model using FP8 precision on 256 Intel Gaudi2 accelerators, achieving on-par results with the BF16 baseline while delivering up to a $\sim 34 \%$ throughput improvement.

FP8로 장기 학습을 진행하면서 발견한 문제. 학습을 일정 이상 진행한 이후에야 아웃라이어가 두드러지게 발생하기 시작하는데 이 아웃라이어가 FP8 학습에 문제를 발생시킨다는 것이죠.

여기서 주목한 것은 SwiGLU입니다. Swish도 일정 이상의 값에 대해서는 거의 선형이므로 게이트 값과 게이트에 곱해지는 값이 잘 정렬되어 있다면 Activation의 크기가 제곱으로 증가하게 되죠. 이것이 아웃라이어를 야기한다고 합니다.

그래서 Scaling Factor를 추가해서 이 문제를 해소했군요. 추가적으로 FP8 State를 사용하는 Adam도 사용해서 2T 학습을 했습니다. 재미있네요.

#efficient-training #quantization 