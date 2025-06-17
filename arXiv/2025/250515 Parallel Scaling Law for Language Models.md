https://arxiv.org/abs/2505.10475

*Parallel Scaling Law for Language Models* (Mouxiang Chen, Binyuan Hui, Zeyu Cui, Jiaxi Yang, Dayiheng Liu, Jianling Sun, Junyang Lin, Zhongxin Liu)

> It is commonly believed that scaling language models should commit a significant space or time cost, by increasing the parameters (parameter scaling) or output tokens (inference-time scaling). We introduce the third and more inference-efficient scaling paradigm: increasing the model's parallel computation during both training and inference time. We apply $P$ diverse and learnable transformations to the input, execute forward passes of the model in parallel, and dynamically aggregate the $P$ outputs. This method, namely parallel scaling (ParScale), scales parallel computation by reusing existing parameters and can be applied to any model structure, optimization procedure, data, or task. We theoretically propose a new scaling law and validate it through large-scale pre-training, which shows that a model with $P$ parallel streams is similar to scaling the parameters by $O(\log P)$ while showing superior inference efficiency. For example, ParScale can use up to 22$\times$ less memory increase and 6$\times$ less latency increase compared to parameter scaling that achieves the same performance improvement. It can also recycle an off-the-shelf pre-trained model into a parallelly scaled one by post-training on a small amount of tokens, further reducing the training budget. The new scaling law we discovered potentially facilitates the deployment of more powerful models in low-resource scenarios, and provides an alternative perspective for the role of computation in machine learning.

변환된 입력들을 Forward한 다음 결합해서 Scaling을 시도한 방법. 변환은 Attention 레이어 입력에 Prefix를 붙이는 방식으로 했습니다. Classifier-Free Guidance를 언급하고 있는데 Test-Time Augmentation도 생각이 나네요.

<english>
Attempt to do scaling by forward transformed inputs and aggregates it. Transformation was done by appending prefix on input of attention layer. While they mentions classifier-free guidance, it also reminds me test-time augmentation.
</english>

#scaling-law #transformer 