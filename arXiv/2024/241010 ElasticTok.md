https://arxiv.org/abs/2410.08368

*ElasticTok: Adaptive Tokenization for Image and Video* (Wilson Yan, Matei Zaharia, Volodymyr Mnih, Pieter Abbeel, Aleksandra Faust, Hao Liu)

> Efficient video tokenization remains a key bottleneck in learning general purpose vision models that are capable of processing long video sequences. Prevailing approaches are restricted to encoding videos to a fixed number of tokens, where too few tokens will result in overly lossy encodings, and too many tokens will result in prohibitively long sequence lengths. In this work, we introduce ElasticTok, a method that conditions on prior frames to adaptively encode a frame into a variable number of tokens. To enable this in a computationally scalable way, we propose a masking technique that drops a random number of tokens at the end of each frames's token encoding. During inference, ElasticTok can dynamically allocate tokens when needed -- more complex data can leverage more tokens, while simpler data only needs a few tokens. Our empirical evaluations on images and video demonstrate the effectiveness of our approach in efficient token usage, paving the way for future development of more powerful multimodal models, world models, and agents.

장면의 인코딩 난이도에 따라 사용하는 토큰 수를 바꾸는 접근. 랜덤한 숫자의 토큰만을 사용하도록 마스킹해서 학습한 다음 추론 시점에는 MSE 같은 지표를 일정 수준 이상 달성할 수 있는 최소의 토큰 수를 찾는 방법을 사용합니다. 재미있네요.

<english>
Approach that changing number of tokens with respect to complexity of scene. Training with random number of tokens with masking, and at the inference time, search is employed to ensure minimizing number of tokens to reach certain level of metrics like MSE. Interesting.
</english>

#vq 