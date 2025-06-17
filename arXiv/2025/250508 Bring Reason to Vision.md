https://arxiv.org/abs/2505.05464

*Bring Reason to Vision: Understanding Perception and Reasoning through Model Merging* (Shiqi Chen, Jinghan Zhang, Tongyao Zhu, Wei Liu, Siyang Gao, Miao Xiong, Manling Li, Junxian He)

> Vision-Language Models (VLMs) combine visual perception with the general capabilities, such as reasoning, of Large Language Models (LLMs). However, the mechanisms by which these two abilities can be combined and contribute remain poorly understood. In this work, we explore to compose perception and reasoning through model merging that connects parameters of different models. Unlike previous works that often focus on merging models of the same kind, we propose merging models across modalities, enabling the incorporation of the reasoning capabilities of LLMs into VLMs. Through extensive experiments, we demonstrate that model merging offers a successful pathway to transfer reasoning abilities from LLMs to VLMs in a training-free manner. Moreover, we utilize the merged models to understand the internal mechanism of perception and reasoning and how merging affects it. We find that perception capabilities are predominantly encoded in the early layers of the model, whereas reasoning is largely facilitated by the middle-to-late layers. After merging, we observe that all layers begin to contribute to reasoning, whereas the distribution of perception abilities across layers remains largely unchanged. These observations shed light on the potential of model merging as a tool for multimodal integration and interpretation.

텍스트 추론 모델과 VLM을 합쳐 이미지 추론 능력을 탑재. 텍스트로 추론 포스트트레이닝을 한 것이 다른 모달리티에도 적용된다는 결과와 유사하겠죠. (https://arxiv.org/abs/2505.03981) 모달리티가 정렬이 잘 되어있다면 자연스러운 결과일 것 같습니다.

<english>
Bringing image reasoning capabilities by merging text reasoning models and VLM. It is similar to the result that doing reasoning post-training only on text can be transferred to another modalities (https://arxiv.org/abs/2505.03981). It would be natural result if modalities well aligned all together.
</english>

#reasoning #multimodal 