https://arxiv.org/abs/2408.08681

*A Mean Field Ansatz for Zero-Shot Weight Transfer* (Xingyuan Chen, Wenwei Kuang, Lei Deng, Wei Han, Bo Bai, Goncalo dos Reis)

> The pre-training cost of large language models (LLMs) is prohibitive. One cutting-edge approach to reduce the cost is zero-shot weight transfer, also known as model growth for some cases, which magically transfers the weights trained in a small model to a large model. However, there are still some theoretical mysteries behind the weight transfer. In this paper, inspired by prior applications of mean field theory to neural network dynamics, we introduce a mean field ansatz to provide a theoretical explanation for weight transfer. Specifically, we propose the row-column (RC) ansatz under the mean field point of view, which describes the measure structure of the weights in the neural network (NN) and admits a close measure dynamic. Thus, the weights of different sizes NN admit a common distribution under proper assumptions, and weight transfer methods can be viewed as sampling methods. We empirically validate the RC ansatz by exploring simple MLP examples and LLMs such as GPT-3 and Llama-3.1. We show the mean-field point of view is adequate under suitable assumptions which can provide theoretical support for zero-shot weight transfer.

작은 모델에서 큰 모델로 Weight Transfer를 하려는 시도. 기본적인 아이디어는 학습된 작은 모델의 Weight에서 Empirical Distribution을 계산한 다음 이 분포로부터 큰 모델에 대한 Weight를 샘플링 하는 접근인 것 같습니다.

#efficient-training 