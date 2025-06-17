https://arxiv.org/abs/2501.09891

*Evolving Deeper LLM Thinking* (Kuang-Huei Lee, Ian Fischer, Yueh-Hua Wu, Dave Marwood, Shumeet Baluja, Dale Schuurmans, Xinyun Chen)

> We explore an evolutionary search strategy for scaling inference time compute in Large Language Models. The proposed approach, Mind Evolution, uses a language model to generate, recombine and refine candidate responses. The proposed approach avoids the need to formalize the underlying inference problem whenever a solution evaluator is available. Controlling for inference cost, we find that Mind Evolution significantly outperforms other inference strategies such as Best-of-N and Sequential Revision in natural language planning tasks. In the TravelPlanner and Natural Plan benchmarks, Mind Evolution solves more than 98% of the problem instances using Gemini 1.5 Pro without the use of a formal solver.

진화 알고리즘을 통한 Inference Time Scaling. Critic을 사용해 생성 텍스트를 개선하는 단계가 들어가는군요. 진화 알고리즘을 통한 프롬프트 최적화 등의 시도가 있었죠. 그런 시도의 연장 같긴 하네요.

<english>
Inference time scaling using evolutionary algorithm. It uses a stage that improves generated texts using critic. There was an approach that uses evolutionary algorithms for the problems like prompt optimization. This seems an extension of that kind of approach.
</english>

#evolutionary-algorithm #inference-time-scaling
