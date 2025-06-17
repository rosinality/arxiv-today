https://arxiv.org/abs/2410.10630

*Thinking LLMs: General Instruction Following with Thought Generation* (Tianhao Wu, Janice Lan, Weizhe Yuan, Jiantao Jiao, Jason Weston, Sainbayar Sukhbaatar)

> LLMs are typically trained to answer user questions or follow instructions similarly to how human experts respond. However, in the standard alignment framework they lack the basic ability of explicit thinking before answering. Thinking is important for complex questions that require reasoning and planning -- but can be applied to any task. We propose a training method for equipping existing LLMs with such thinking abilities for general instruction following without use of additional human data. We achieve this by an iterative search and optimization procedure that explores the space of possible thought generations, allowing the model to learn how to think without direct supervision. For each instruction, the thought candidates are scored using a judge model to evaluate their responses only, and then optimized via preference optimization. We show that this procedure leads to superior performance on AlpacaEval and Arena-Hard, and shows gains from thinking on non-reasoning categories such as marketing, health and general knowledge, in addition to more traditional reasoning & problem-solving tasks.

일반적인 Instruction Following 능력에 생각을 하는 과정을 추가. 생각을 생성하도록 프롬프트를 사용한 다음 생각을 제외한 최종 결과만 Reward Model로 평가하게 하는 형태로 진행. 

<english>
Adding thinking process to general instruction following capabilities. Let model to generate thinking using prompt and let reward model to judge final response excpet thoughts.
</english>

#instruction-tuning #reasoning 