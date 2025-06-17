https://arxiv.org/abs/2401.17464

*Efficient Tool Use with Chain-of-Abstraction Reasoning* (Silin Gao, Jane Dwivedi-Yu, Ping Yu, Xiaoqing Ellen Tan, Ramakanth Pasunuru, Olga Golovneva, Koustuv Sinha, Asli Celikyilmaz, Antoine Bosselut, Tianlu Wang)

> To achieve faithful reasoning that aligns with human expectations, large language models (LLMs) need to ground their reasoning to real-world knowledge (e.g., web facts, math and physical rules). Tools help LLMs access this external knowledge, but there remains challenges for fine-tuning LLM agents (e.g., Toolformer) to invoke tools in multi-step reasoning problems, where inter-connected tool calls require holistic and efficient tool usage planning. In this work, we propose a new method for LLMs to better leverage tools in multi-step reasoning. Our method, Chain-of-Abstraction (CoA), trains LLMs to first decode reasoning chains with abstract placeholders, and then call domain tools to reify each reasoning chain by filling in specific knowledge. This planning with abstract chains enables LLMs to learn more general reasoning strategies, which are robust to shifts of domain knowledge (e.g., math results) relevant to different reasoning questions. It also allows LLMs to perform decoding and calling of external tools in parallel, which avoids the inference delay caused by waiting for tool responses. In mathematical reasoning and Wiki QA domains, we show that our method consistently outperforms previous chain-of-thought and tool-augmented baselines on both in-distribution and out-of-distribution test sets, with an average ~6% absolute QA accuracy improvement. LLM agents trained with our method also show more efficient tool use, with inference speed being on average ~1.4x faster than baseline tool-augmented LLMs.

생각과 도구 실행을 반복하는 것이 아니라 계획을 만들어서 실행시키는 방법. 예를 들어 20 + 35 = 55, 90 - 55 = 35 같은 연산을 나눠서 수행하는 것이 아니라 20 + 35 = y1, 90 - y1 = y2 같은 식으로 계획을 만들어 수행하는 것이죠. (깨알 같이 x, y, z를 쓰는 것보다 y1, y2를 쓰는 것이 나았다고 하네요.)

전반적으로 LLM Compiler (https://arxiv.org/abs/2312.04511) 가 떠오르는군요.

#tool 

Instead of using interleaved chains of thought and tool execution, build tool use plans and execute it. For example, instead of separated sequences of tool use like 25 + 35 = 55, 90 - 55 = 35, make a plan of 20 + 35 = y1, 90 - y1 = y2. (It is small tips for use y1, y2 instead of x, y, z).

Overall it reminds me LLM Compiler.

# Links

[[231207 An LLM Compiler for Parallel Function Calling.md]]