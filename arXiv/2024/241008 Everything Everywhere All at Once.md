https://arxiv.org/abs/2410.05603

*Everything Everywhere All at Once: LLMs can In-Context Learn Multiple Tasks in Superposition* (Zheyang Xiong, Ziyang Cai, John Cooper, Albert Ge, Vasilis Papageorgiou, Zack Sifakis, Angeliki Giannou, Ziqian Lin, Liu Yang, Saurabh Agarwal, Grigorios G Chrysos, Samet Oymak, Kangwook Lee, Dimitris Papailiopoulos)

> Large Language Models (LLMs) have demonstrated remarkable in-context learning (ICL) capabilities. In this study, we explore a surprising phenomenon related to ICL: LLMs can perform multiple, computationally distinct ICL tasks simultaneously, during a single inference call, a capability we term "task superposition". We provide empirical evidence of this phenomenon across various LLM families and scales and show that this phenomenon emerges even if we train the model to in-context learn one task at a time. We offer theoretical explanations that this capability is well within the expressive power of transformers. We also explore how LLMs internally compose task vectors during superposition. Furthermore, we show that larger models can solve more ICL tasks in parallel, and better calibrate their output distribution. Our findings offer insights into the latent capabilities of LLMs, further substantiate the perspective of "LLMs as superposition of simulators", and raise questions about the mechanisms enabling simultaneous task execution.

In-context Learning에서 여러 과제를 수행하도록 예제를 섞었을 때에도 그 과제들을 모두 반영할 수 있다는 결과. 심지어 하나의 과제만 수행하도록 학습한 경우에도 여러 과제에 대한 대응이 가능했다고 하네요.

<english>
The result that model can reflect each of all of the tasks in in-context learning, even when multiple tasks are mixed. Surprisingly it is possible to deal with multiple tasks even trained with single tasks.
</english>

#in-context-learning 