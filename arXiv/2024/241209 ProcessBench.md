https://arxiv.org/abs/2412.06559

*ProcessBench: Identifying Process Errors in Mathematical Reasoning* (Chujie Zheng, Zhenru Zhang, Beichen Zhang, Runji Lin, Keming Lu, Bowen Yu, Dayiheng Liu, Jingren Zhou, Junyang Lin)

> As language models regularly make mistakes when solving math problems, automated identification of errors in the reasoning process becomes increasingly significant for their scalable oversight. In this paper, we introduce ProcessBench for measuring the ability to identify erroneous steps in mathematical reasoning. It consists of 3,400 test cases, primarily focused on competition- and Olympiad-level math problems. Each test case contains a step-by-step solution with error location annotated by human experts. Models are required to identify the earliest step that contains an error, or conclude that all steps are correct. We conduct extensive evaluation on ProcessBench, involving two types of models: process reward models (PRMs) and critic models, where for the latter we prompt general language models to critique each solution step by step. We draw two main observations: (1) Existing PRMs typically fail to generalize to more challenging math problems beyond GSM8K and MATH. They underperform both critic models (i.e., prompted general language models) and our own trained PRM that is straightforwardly fine-tuned on the PRM800K dataset. (2) The best open-source model, QwQ-32B-Preview, has demonstrated the critique capability competitive with the proprietary model GPT-4o, despite that it still lags behind the reasoning-specialized o1-mini. We hope ProcessBench can foster future research in reasoning process assessment, paving the way toward scalable oversight of language models.

Process Reward 모델과 Critic 모델을 위한 벤치마크. GSM8K, MATH, OlympiadBench, Omni-MATH의 문제들에 대해 LLM으로 정답을 생성하고 사람이 오류가 발생한 지점을 어노테이션하는 방식으로 구축했네요.

PRM의 경우에는 학습에 사용한 데이터 분포의 차이와 정답의 정확성으로 과정의 정확성을 평가하는 방법의 한계로 성능에 문제가 있네요. 프롬프팅한 Critic 모델에도 밀리는 결과가 나타납니다. 그냥 PRM800K로 학습한 모델이 가장 나았다고 합니다. 

Critic 모델의 경우에는, 특히 추론 모델의 경우에는 추론 과정을 통해 더 나은 성능에 도달할 수 있었다고 하네요.

그렇다면 QwQ는 어떻게 만든 걸까요.

<english>
A benchmark for process reward and critic models. They generated solutions using LLMs for problems in GSM8K, MATH, OlympiadBench, Omni-MATH, and annotated the point where error occurs by human.

For PRM it has a problem in the performance because of difference in distribution that is used for the training and limitation of evaluating accuracy of the process just by correctness of the answer. It is below of prompted critic models. For PRM the model trained just with PRM800K was the best.

For critic models, especially reasoning models, it was possible to reach better performances by separated reasoning processes.

Then how they did make QwQ?
</english>

#reward-model #reasoning #math #benchmark 