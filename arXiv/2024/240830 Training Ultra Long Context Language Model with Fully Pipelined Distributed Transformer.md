https://arxiv.org/abs/2408.16978

*Training Ultra Long Context Language Model with Fully Pipelined Distributed Transformer* (Jinghan Yao, Sam Ade Jacobs, Masahiro Tanaka, Olatunji Ruwase, Aamir Shafi, Hari Subramoni, Dhabaleswar K. Panda)

> Large Language Models (LLMs) with long context capabilities are integral to complex tasks in natural language processing and computational biology, such as text generation and protein sequence analysis. However, training LLMs directly on extremely long contexts demands considerable GPU resources and increased memory, leading to higher costs and greater complexity. Alternative approaches that introduce long context capabilities via downstream finetuning or adaptations impose significant design limitations. In this paper, we propose Fully Pipelined Distributed Transformer (FPDT) for efficiently training long-context LLMs with extreme hardware efficiency. For GPT and Llama models, we achieve a 16x increase in sequence length that can be trained on the same hardware compared to current state-of-the-art solutions. With our dedicated sequence chunk pipeline design, we can now train 8B LLM with 2 million sequence length on only 4 GPUs, while also maintaining over 55% of MFU. Our proposed FPDT is agnostic to existing training techniques and is proven to work efficiently across different LLM models.

Long Context Attention 구현. DeepSpeed Ulysses와 비슷한 All-to-All 기반의 헤드 쪼개기인데 추가적으로 시퀀스 또한 쪼개는군요. 쪼갠 시퀀스들에 대해 Online Attention을 계산하면서 Backprop에 필요한 텐서들을 CPU Offloading을 합니다.

#long-context #efficient-training 