https://arxiv.org/abs/2504.08719

*SWAN-GPT: An Efficient and Scalable Approach for Long-Context Language Modeling* (Krishna C. Puvvada, Faisal Ladhak, Santiago Akle Serrano, Cheng-Ping Hsieh, Shantanu Acharya, Somshubra Majumdar, Fei Jia, Samuel Kriman, Simeng Sun, Dima Rekesh, Boris Ginsburg)

> We present a decoder-only Transformer architecture that robustly generalizes to sequence lengths substantially longer than those seen during training. Our model, SWAN-GPT, interleaves layers without positional encodings (NoPE) and sliding-window attention layers equipped with rotary positional encodings (SWA-RoPE). Experiments demonstrate strong performance on sequence lengths significantly longer than the training length without the need for additional long-context training. This robust length extrapolation is achieved through our novel architecture, enhanced by a straightforward dynamic scaling of attention scores during inference. In addition, SWAN-GPT is more computationally efficient than standard GPT architectures, resulting in cheaper training and higher throughput. Further, we demonstrate that existing pre-trained decoder-only models can be efficiently converted to the SWAN architecture with minimal continued training, enabling longer contexts. Overall, our work presents an effective approach for scaling language models to longer contexts in a robust and efficient manner.

Window Attention + RoPE와 Global Attention + NoPE, 그리고 Attention Logit Scaling을 사용한 Length Generalization. Llama 4의 세팅이죠. 이 세팅이 얼마나 효과적인지는 Llama 4를 통해서 확인할 수 있겠죠.

<english>
A length generalization method based on window attention + RoPE and global attention + NoPE, and attention logit scaling. It is exactly settings of Llama 4. We would able to confirm effectiveness of this settings through Llama 4.
</english>

#long-context #positional-encoding 