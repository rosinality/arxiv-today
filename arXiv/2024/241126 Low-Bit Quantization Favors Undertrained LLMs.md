https://arxiv.org/abs/2411.17691

*Low-Bit Quantization Favors Undertrained LLMs: Scaling Laws for Quantized LLMs with 100T Training Tokens* (Xu Ouyang, Tao Ge, Thomas Hartvigsen, Zhisong Zhang, Haitao Mi, Dong Yu)

> We reveal that low-bit quantization favors undertrained large language models (LLMs) by observing that models with larger sizes or fewer training tokens experience less quantization-induced degradation (QiD) when applying low-bit quantization, whereas smaller models with extensive training tokens suffer significant QiD. To gain deeper insights into this trend, we study over 1500 quantized LLM checkpoints of various sizes and at different training levels (undertrained or fully trained) in a controlled setting, deriving scaling laws for understanding the relationship between QiD and factors such as the number of training tokens, model size and bit width. With the derived scaling laws, we propose a novel perspective that we can use QiD to measure an LLM's training levels and determine the number of training tokens required for fully training LLMs of various sizes. Moreover, we use the scaling laws to predict the quantization performance of different-sized LLMs trained with 100 trillion tokens. Our projection shows that the low-bit quantization performance of future models, which are expected to be trained with over 100 trillion tokens, may NOT be desirable. This poses a potential challenge for low-bit quantization in the future and highlights the need for awareness of a model's training level when evaluating low-bit quantization research. To facilitate future research on this problem, we release all the 1500+ quantized checkpoints used in this work at https://huggingface.co/Xu-Ouyang.

Quantization으로 인해 발생하는 손실에 대한 Scaling Law. Quantization 이후와 이전의 Loss 차이가 학습 토큰 수에 비례하고 모델 크기와 Precision에 반비례한다는 형태입니다. (https://arxiv.org/abs/2411.04330) 결과적으로 Quantization에 대해서는 Undertrain된 모델이 더 선호된다는 것이죠. 파레토 최적 지점이 궁금하네요.

조금 다른 아이디어인데 Loss의 차이가 작다면 Undertrain 되었다고 생각할 수 있고 반대로 어느 정도까지 더 학습을 시킬 수 있는가를 추정할 수 있지 않을까 하는 이야기를 합니다.

<english>
Scaling law for loss difference due to quantization. Overall formula is loss difference between after and before quantization is proportional to training tokens and inversely proportional to model sizes and precision. (https://arxiv.org/abs/2411.04330) So for quantization undertrained is more preferred. I wonder what is the pareto optimal point.

Slightly different idea is also suggested. We can think if loss difference is small then model is undertrained. So reversely, maybe we can estimate how further we can train the model from it.
</english>

#quantization #scaling-law

# Links

[[241107 Scaling Laws for Precision.md]]