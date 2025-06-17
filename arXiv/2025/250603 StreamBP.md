https://arxiv.org/abs/2506.03077

*StreamBP: Memory-Efficient Exact Backpropagation for Long Sequence Training of LLMs* (Qijun Luo, Mengqi Li, Lei Zhao, Xiao Li)

> Training language models on long sequence data is a demanding requirement for enhancing the model's capability on complex tasks, e.g., long-chain reasoning. However, as the sequence length scales up, the memory cost for storing activation values becomes huge during the Backpropagation (BP) process, even with the application of gradient checkpointing technique. To tackle this challenge, we propose a memory-efficient and exact BP method called StreamBP, which performs a linear decomposition of the chain rule along the sequence dimension in a layer-wise manner, significantly reducing the memory cost of activation values and logits. The proposed method is applicable to common objectives such as SFT, GRPO, and DPO. From an implementation perspective, StreamBP achieves less computational FLOPs and faster BP speed by leveraging the causal structure of the language model. Compared to gradient checkpointing, StreamBP scales up the maximum sequence length of BP by 2.8-5.5 times larger, while using comparable or even less BP time. Note that StreamBP's sequence length scaling ability can be directly transferred to batch size scaling for accelerating training. We further develop a communication-efficient distributed StreamBP to effectively support multi-GPU training and broaden its applicability. Our code can be easily integrated into the training pipeline of any transformer models and is available at https://github.com/Ledzy/StreamBP.

시퀀스 방향으로 입력을 쪼개서 순차적으로 Backprop을 하는 방법. 이전의 Blockwise Transformer가 생각나네요 (https://arxiv.org/abs/2305.19370).

<english>
Sequentially doing backprop by chunking the input along sequence direction. It reminds me previous study of blockwise transformer (https://arxiv.org/abs/2305.19370).
</english>

#efficiency #long-context #transformer 