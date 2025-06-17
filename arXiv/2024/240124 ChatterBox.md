https://arxiv.org/abs/2401.13307

*ChatterBox: Multi-round Multimodal Referring and Grounding* (Yunjie Tian, Tianren Ma, Lingxi Xie, Jihao Qiu, Xi Tang, Yuan Zhang, Jianbin Jiao, Qi Tian, Qixiang Ye)

> In this study, we establish a baseline for a new task named multimodal multi-round referring and grounding (MRG), opening up a promising direction for instance-level multimodal dialogues. We present a new benchmark and an efficient vision-language model for this purpose. The new benchmark, named CB-300K, spans challenges including multi-round dialogue, complex spatial relationships among multiple instances, and consistent reasoning, which are beyond those shown in existing benchmarks. The proposed model, named ChatterBox, utilizes a two-branch architecture to collaboratively handle vision and language tasks. By tokenizing instance regions, the language branch acquires the ability to perceive referential information. Meanwhile, ChatterBox feeds a query embedding in the vision branch to a token receiver for visual grounding. A two-stage optimization strategy is devised, making use of both CB-300K and auxiliary external data to improve the model's stability and capacity for instance-level understanding. Experiments show that ChatterBox outperforms existing models in MRG both quantitatively and qualitatively, paving a new path towards multimodal dialogue scenarios with complicated and precise interactions. Code, data, and model are available at: https://github.com/sunsmarterjie/ChatterBox.

멀티 턴 Visual Grounding과 Referring에 대한 데이터셋. Visual Genome 데이터셋의 BBox와 Relationship, 객체의 속성을 기반으로 GPT-4로 질문과 답을 만들고, 다음 질문이 이전 질문을 기반으로 하도록 해서 만들었습니다.

기존에 구축되어 있는 데이터셋들이 꽤 있으니 그걸 채택하거나 변형해서 새로운 과제를 만들어 학습시키는 것으로 Vision-Language와 관련된 능력을 향상시키는 것도 꽤 좋은 방향일 듯 싶습니다.

#dataset #vision-language #instruction-tuning #visual_grounding #benchmark 