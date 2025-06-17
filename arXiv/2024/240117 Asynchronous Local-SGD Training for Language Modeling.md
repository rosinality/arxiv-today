https://arxiv.org/abs/2401.09135

*Asynchronous Local-SGD Training for Language Modeling* (Bo Liu, Rachita Chhaparia, Arthur Douillard, Satyen Kale, Andrei A. Rusu, Jiajun Shen, Arthur Szlam, Marc'Aurelio Ranzato)

> Local stochastic gradient descent (Local-SGD), also referred to as federated averaging, is an approach to distributed optimization where each device performs more than one SGD update per communication. This work presents an empirical study of {\it asynchronous} Local-SGD for training language models; that is, each worker updates the global parameters as soon as it has finished its SGD steps. We conduct a comprehensive investigation by examining how worker hardware heterogeneity, model size, number of workers, and optimizer could impact the learning performance. We find that with naive implementations, asynchronous Local-SGD takes more iterations to converge than its synchronous counterpart despite updating the (global) model parameters more frequently. We identify momentum acceleration on the global parameters when worker gradients are stale as a key challenge. We propose a novel method that utilizes a delayed Nesterov momentum update and adjusts the workers' local training steps based on their computation speed. This approach, evaluated with models up to 150M parameters on the C4 dataset, matches the performance of synchronous Local-SGD in terms of perplexity per update step, and significantly surpasses it in terms of wall clock time.

구글은 Local, Async SGD를 계속 실험해보는군요. (Local SGD를 해봤으니 Async도 해보자 정도의 발상일 수도 있겠습니다.) Gemini에서도 데이터센터를 연결해서 학습했다는 걸 생각해보면 이 계통 방법이 매력적으로 보일 수도 있겠다 싶습니다.

여기서는 Async + Local 세팅에서 이유는 잘 모르겠지만 Outer Loop의 모멘텀 업데이트 과정에서 문제가 생긴다는 것으로 보고 모멘텀 업데이트의 횟수를 줄이는 방식으로 대응했습니다.

실험 규모도 작고 더 큰 모델에서 어떤 문제가 터질지 모르겠지만 만약 성공적으로 적용할 수 있다면 가뜩이나 많은 연산력이 다시 한 번 부스트 되는 효과가 있겠네요.

#efficient_training 