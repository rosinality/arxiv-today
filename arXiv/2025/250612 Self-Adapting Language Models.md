https://arxiv.org/abs/2506.10943

*Self-Adapting Language Models* (Adam Zweiger, Jyothish Pari, Han Guo, Ekin Akyürek, Yoon Kim, Pulkit Agrawal)

> Large language models (LLMs) are powerful but static; they lack mechanisms to adapt their weights in response to new tasks, knowledge, or examples. We introduce Self-Adapting LLMs (SEAL), a framework that enables LLMs to self-adapt by generating their own finetuning data and update directives. Given a new input, the model produces a self-edit-a generation that may restructure the information in different ways, specify optimization hyperparameters, or invoke tools for data augmentation and gradient-based updates. Through supervised finetuning (SFT), these self-edits result in persistent weight updates, enabling lasting adaptation. To train the model to produce effective self-edits, we use a reinforcement learning loop with the downstream performance of the updated model as the reward signal. Unlike prior approaches that rely on separate adaptation modules or auxiliary networks, SEAL directly uses the model's own generation to control its adaptation process. Experiments on knowledge incorporation and few-shot generalization show that SEAL is a promising step toward language models capable of self-directed adaptation. Our website and code is available at https://jyopari.github.io/posts/seal.

모델이 스스로를 개선하도록 학습. 새로운 과제에 대해서 학습할 데이터를 모델이 만들게 하고 그 데이터로 학습한 결과를 보상으로 해서 모델을 학습시키는 형태군요. 메타러닝이네요.

<english>
Training model to improve itself. First let model to generate training data for novel tasks, and training model using the result from training on that data as a result. It is meta-learning.
</english>

#meta-learning 