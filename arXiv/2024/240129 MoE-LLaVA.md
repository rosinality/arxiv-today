https://arxiv.org/abs/2401.15947

*MoE-LLaVA: Mixture of Experts for Large Vision-Language Models* (Bin Lin, Zhenyu Tang, Yang Ye, Jiaxi Cui, Bin Zhu, Peng Jin, Junwu Zhang, Munan Ning, Li Yuan)

> For Large Vision-Language Models (LVLMs), scaling the model can effectively improve performance. However, expanding model parameters significantly increases the training and inferring costs, as all model parameters are activated for each token in the calculation. In this work, we propose a novel training strategy MoE-tuning for LVLMs, which can constructing a sparse model with an outrageous number of parameter but a constant computational cost, and effectively addresses the performance degradation typically associated with multi-modal learning and model sparsity. Furthermore, we present the MoE-LLaVA framework, a MoE-based sparse LVLM architecture. This framework uniquely activates only the top-k experts through routers during deployment, keeping the remaining experts inactive. Our extensive experiments highlight the excellent capabilities of MoE-LLaVA in visual understanding and its potential to reduce hallucinations in model outputs. Remarkably, with just 3 billion sparsely activated parameters, MoE-LLaVA demonstrates performance comparable to the LLaVA-1.5-7B on various visual understanding datasets and even surpasses the LLaVA-1.5-13B in object hallucination benchmarks. Through MoE-LLaVA, we aim to establish a baseline for sparse LVLMs and provide valuable insights for future research in developing more efficient and effective multi-modal learning systems. Code is released at \url{https://github.com/PKU-YuanGroup/MoE-LLaVA}.

Projector Tuning -> Full Finetuning -> FFN 복붙으로 MoE Tuning의 3단 튜닝으로 만들어진 VLM. MoE를 할 수 있다면 하지 않을 이유가 없는 상황이 됐군요.

이미지와 텍스트 토큰의 Expert Assignment를 봤을 때 각 Expert에 이미지와 텍스트가 비슷한 비율로 들어가는 것이 흥미로운 부분이군요. 즉 이미지 전담 Expert가 있는 것이 아니라 한 Expert가 이미지와 텍스트를 동시에 커버한다는 의미입니다.

#moe #vision-language 

3 staged training of VLMs with Projector Tuning -> Full Finetuning -> MoE Tuning by copy-pasting FFNs. It seems that there are no reason for avoiding MoEs if you can train and deploy it.

It is worth notice that ration of image and text token inputs for each experts are similar, as shown in expert assignment. That is, there are no "Image Experts" or "Text Experts". Instead each expert accepts image and text tokens simultaneously.