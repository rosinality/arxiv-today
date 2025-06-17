https://arxiv.org/abs/2402.04792

*Direct Language Model Alignment from Online AI Feedback* (Shangmin Guo, Biao Zhang, Tianlin Liu, Tianqi Liu, Misha Khalman, Felipe Llinares, Alexandre Rame, Thomas Mesnard, Yao Zhao, Bilal Piot, Johan Ferret, Mathieu Blondel)

> Direct alignment from preferences (DAP) methods, such as DPO, have recently emerged as efficient alternatives to reinforcement learning from human feedback (RLHF), that do not require a separate reward model. However, the preference datasets used in DAP methods are usually collected ahead of training and never updated, thus the feedback is purely offline. Moreover, responses in these datasets are often sampled from a language model distinct from the one being aligned, and since the model evolves over training, the alignment phase is inevitably off-policy. In this study, we posit that online feedback is key and improves DAP methods. Our method, online AI feedback (OAIF), uses an LLM as annotator: on each training iteration, we sample two responses from the current model and prompt the LLM annotator to choose which one is preferred, thus providing online feedback. Despite its simplicity, we demonstrate via human evaluation in several tasks that OAIF outperforms both offline DAP and RLHF methods. We further show that the feedback leveraged in OAIF is easily controllable, via instruction prompts to the LLM annotator.

DPO 같은 방법이 실질적으로 Policy가 아닌 다른 모델이 생성한 샘플을 한 번 어노테이션한 데이터셋에 대해 지속적으로 학습하는 형태로 사용되고 있다는 문제 의식. 단순하게 Policy로 샘플링하고, LLM으로 어노테이션하고, 그 결과로 학습하는 루프로 학습시키는 방법을 채택했습니다.

#rlaif #alignment