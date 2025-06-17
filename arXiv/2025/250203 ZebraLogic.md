https://arxiv.org/abs/2502.01100

*ZebraLogic: On the Scaling Limits of LLMs for Logical Reasoning* (Bill Yuchen Lin, Ronan Le Bras, Kyle Richardson, Ashish Sabharwal, Radha Poovendran, Peter Clark, Yejin Choi)

> We investigate the logical reasoning capabilities of large language models (LLMs) and their scalability in complex non-monotonic reasoning. To this end, we introduce ZebraLogic, a comprehensive evaluation framework for assessing LLM reasoning performance on logic grid puzzles derived from constraint satisfaction problems (CSPs). ZebraLogic enables the generation of puzzles with controllable and quantifiable complexity, facilitating a systematic study of the scaling limits of models such as Llama, o1 models, and DeepSeek-R1. By encompassing a broad range of search space complexities and diverse logical constraints, ZebraLogic provides a structured environment to evaluate reasoning under increasing difficulty. Our results reveal a significant decline in accuracy as problem complexity grows -- a phenomenon we term the curse of complexity. This limitation persists even with larger models and increased inference-time computation, suggesting inherent constraints in current LLM reasoning capabilities. Additionally, we explore strategies to enhance logical reasoning, including Best-of-N sampling, backtracking mechanisms, and self-verification prompts. Our findings offer critical insights into the scalability of LLM reasoning, highlight fundamental limitations, and outline potential directions for improvement.

논리 퍼즐을 생성해 구축한 벤치마크. 논리 문제는 평가에 더해 생성을 고려할 수 있는 분야죠. (https://arxiv.org/abs/2411.12498) 추론 학습에 쓸 수 있을지도 모르겠네요.

<english>
Benchmark constructed by synthesized logic puzzles. Logic problem is a domain we can consider generation in addition to evaluation (https://arxiv.org/abs/2411.12498). Maybe we can use it for training reasoning models.
</english>

#reasoning #synthetic-data #benchmark

# Links

[[241119 Enhancing Reasoning Capabilities of LLMs via Principled Synthetic Logic Corpus.md]]