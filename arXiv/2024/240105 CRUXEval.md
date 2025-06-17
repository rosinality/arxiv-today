https://arxiv.org/abs/2401.03065

*CRUXEval: A Benchmark for Code Reasoning, Understanding and Execution* (Alex Gu, Baptiste Rozière, Hugh Leather, Armando Solar-Lezama, Gabriel Synnaeve, Sida I. Wang)

> We present CRUXEval (Code Reasoning, Understanding, and eXecution Evaluation), a benchmark consisting of 800 Python functions (3-13 lines). Each function comes with an input-output pair, leading to two natural tasks: input prediction and output prediction. First, we propose a generic recipe for generating our execution benchmark which can be used to create future variation of the benchmark. Second, we evaluate twenty code models on our benchmark and discover that many recent high-scoring models on HumanEval do not show the same improvements on our benchmark. Third, we show that simple CoT and fine-tuning schemes can improve performance on our benchmark but remain far from solving it. The best setup, GPT-4 with chain of thought (CoT), achieves a pass@1 of 75% and 81% on input and output prediction, respectively. In contrast, Code Llama 34B achieves a pass@1 of 50% and 46% on input and output prediction, highlighting the gap between open and closed source models. As no model is close to acing CRUXEval, we provide examples of consistent GPT-4 failures on simple programs as a lens into its code reasoning capabilities and areas for improvement.

코드 벤치마크가 하나 나왔군요. 함수를 주고 주어진 입력에 대한 출력 예측 혹은 주어진 출력에 대한 입력을 예측하는 과제입니다. GPT-3.5와 다른 코드 모델들 사이의 갭은 꽤 줄어든 것 같은데 GPT-4는 여전히 압도적이군요

#benchmark #code 