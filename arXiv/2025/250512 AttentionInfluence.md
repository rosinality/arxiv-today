https://arxiv.org/abs/2505.07293

*AttentionInfluence: Adopting Attention Head Influence for Weak-to-Strong Pretraining Data Selection* (Kai Hua, Steven Wu, Ge Zhang, Ke Shen)

> Recently, there has been growing interest in collecting reasoning-intensive pretraining data to improve LLMs' complex reasoning ability. Prior approaches typically rely on supervised classifiers to identify such data, which requires labeling by humans or LLMs, often introducing domain-specific biases. Due to the attention heads being crucial to in-context reasoning, we propose AttentionInfluence, a simple yet effective, training-free method without supervision signal. Our approach enables a small pretrained language model to act as a strong data selector through a simple attention head masking operation. Specifically, we identify retrieval heads and compute the loss difference when masking these heads. We apply AttentionInfluence to a 1.3B-parameter dense model to conduct data selection on the SmolLM corpus of 241B tokens, and mix the SmolLM corpus with the selected subset comprising 73B tokens to pretrain a 7B-parameter dense model using 1T training tokens and WSD learning rate scheduling. Our experimental results demonstrate substantial improvements, ranging from 1.4pp to 3.5pp, across several knowledge-intensive and reasoning-heavy benchmarks (i.e., MMLU, MMLU-Pro, AGIEval-en, GSM8K, and HumanEval). This demonstrates an effective weak-to-strong scaling property, with small models improving the final performance of larger models-offering a promising and scalable path for reasoning-centric data selection.

Retrieval Head 같이 추론 능력에 중요한 헤드를 마스킹했을 때와 아닐 때의 Loss 차이를 사용해서 추론 능력에 도움이 되는 데이터를 찾아낸다는 아이디어.

<english>
Find out the data that useful for reasoning abilities, by using difference of losses of when heads like retrieval heads which is important for reasoning abilities are masked or not.
</english>

#reasoning #mechanistic-interpretation #corpus 