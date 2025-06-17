https://arxiv.org/abs/2403.06963

*The pitfalls of next-token prediction* (Gregor Bachmann, Vaishnavh Nagarajan)

> Can a mere next-token predictor faithfully model human intelligence? We crystallize this intuitive concern, which is fragmented in the literature. As a starting point, we argue that the two often-conflated phases of next-token prediction -- autoregressive inference and teacher-forced training -- must be treated distinctly. The popular criticism that errors can compound during autoregressive inference, crucially assumes that teacher-forcing has learned an accurate next-token predictor. This assumption sidesteps a more deep-rooted problem we expose: in certain classes of tasks, teacher-forcing can simply fail to learn an accurate next-token predictor in the first place. We describe a general mechanism of how teacher-forcing can fail, and design a minimal planning task where both the Transformer and the Mamba architecture empirically fail in that manner -- remarkably, despite the task being straightforward to learn. We provide preliminary evidence that this failure can be resolved when training to predict multiple tokens in advance. We hope this finding can ground future debates and inspire explorations beyond the next-token prediction paradigm. We make our code available under https://github.com/gregorbachmann/Next-Token-Failures

Teacher Forcing에서 발생하는 문제. 이전 스텝의 시퀀스들이 정답에 대한 지나치게 많은 정보를 주는 경우에 실제 문제를 푸는 알고리즘이 아니라 이 정보를 이용하는 패턴을 학습할 수 있다는 아이디어. 그렇다면 이 정보를 가리고 토큰을 여러 개 예측하게 하면 되지 않을까 하는 생각으로 이어집니다.

여러모로 Autoregressive / Next Token Prediction은 생각보다 쉽다는 것이 문제가 아닐까 하는 생각이 드네요.

#autoregressive-model