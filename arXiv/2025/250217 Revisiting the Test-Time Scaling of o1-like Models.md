https://arxiv.org/abs/2502.12215

*Revisiting the Test-Time Scaling of o1-like Models: Do they Truly Possess Test-Time Scaling Capabilities?* (Zhiyuan Zeng, Qinyuan Cheng, Zhangyue Yin, Yunhua Zhou, Xipeng Qiu)

> The advent of test-time scaling in large language models (LLMs), exemplified by OpenAI's o1 series, has advanced reasoning capabilities by scaling computational resource allocation during inference. While successors like QwQ, Deepseek-R1 (R1) and LIMO replicate these advancements, whether these models truly possess test-time scaling capabilities remains underexplored. This study found that longer CoTs of these o1-like models do not consistently enhance accuracy; in fact, correct solutions are often shorter than incorrect ones for the same questions. Further investigation shows this phenomenon is closely related to models' self-revision capabilities - longer CoTs contain more self-revisions, which often lead to performance degradation. We then compare sequential and parallel scaling strategies on QwQ, R1 and LIMO, finding that parallel scaling achieves better coverage and scalability. Based on these insights, we propose Shortest Majority Vote, a method that combines parallel scaling strategies with CoT length characteristics, significantly improving models' test-time scalability compared to conventional majority voting approaches.

사고의 길이와 정답률의 관계 문제에 대한 분석. 같은 문제에 대해서도 정답인 경우가 오답인 경우보다 사고의 길이가 짧다고 하는군요. 사고의 길이를 늘리는 주요한 원인은 그다지 효과적이지 않은 Revision을 하기 때문이라고 합니다.

Revision은 참 학습시키기 어려운 능력 중 하나네요. 어쩌면 자신의 생성 결과가 다시 증거가 되는 Autoregression의 기본적인 문제에 기원하는 것일지도 모르겠습니다.

<english>
Analysis on length of reasoning and rate of correct answers. The authors say that correct answers are shorter than incorrect answers in average for same questions. One of cause increases length of reasoning is model does ineffective revision.

Revision is hard capabilities to be trained. Maybe it originates from the fundamental problem of autoregression that its own generation became an evidence.
</english>

#reasoning #inference-time-scaling 