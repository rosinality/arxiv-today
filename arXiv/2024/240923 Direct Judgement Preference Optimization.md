https://arxiv.org/abs/2409.14664

*Direct Judgement Preference Optimization* (Peifeng Wang, Austin Xu, Yilun Zhou, Caiming Xiong, Shafiq Joty)

> Auto-evaluation is crucial for assessing response quality and offering feedback for model development. Recent studies have explored training large language models (LLMs) as generative judges to evaluate and critique other models' outputs. In this work, we investigate the idea of learning from both positive and negative data with preference optimization to enhance the evaluation capabilities of LLM judges across an array of different use cases. We achieve this by employing three approaches to collect the preference pairs for different use cases, each aimed at improving our generative judge from a different perspective. Our comprehensive study over a wide range of benchmarks demonstrates the effectiveness of our method. In particular, our generative judge achieves the best performance on 10 out of 13 benchmarks, outperforming strong baselines like GPT-4o and specialized judge models. Further analysis show that our judge model robustly counters inherent biases such as position and length bias, flexibly adapts to any evaluation protocol specified by practitioners, and provides helpful language feedback for improving downstream generator models.

응답에 대한 평가 모델에 CoT를 결합. 얼마 전에 Reward Model에 대해 비슷한 시도를 한 사례가 있었죠. (https://arxiv.org/abs/2408.11791) CoT 없이 평가, 그리고 평가 결과에 대해 응답을 추측하게 하는 과제를 결합한 다음 DPO로 학습. Teacher 모델의 크기나 Teacher 모델이 생성한 결과가 정답과 일치하는지를 통해 Positive/Negative를 설정합니다.

#reward-model

# Links

[[240821 Critique-out-Loud Reward Models.md]]