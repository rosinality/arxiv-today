https://arxiv.org/abs/2402.07865

*Prismatic VLMs: Investigating the Design Space of Visually-Conditioned Language Models* (Siddharth Karamcheti, Suraj Nair, Ashwin Balakrishna, Percy Liang, Thomas Kollar, Dorsa Sadigh)

> Visually-conditioned language models (VLMs) have seen growing adoption in applications such as visual dialogue, scene understanding, and robotic task planning; adoption that has fueled a wealth of new models such as LLaVa, InstructBLIP, and PaLI-3. Despite the volume of new releases, key design decisions around image preprocessing, architecture, and optimization are under-explored, making it challenging to understand what factors account for model performance $-$ a challenge further complicated by the lack of objective, consistent evaluations. To address these gaps, we first compile a suite of standardized evaluations spanning visual question answering, object localization from language, and targeted challenge sets that probe properties such as hallucination; evaluations that provide calibrated, fine-grained insight into a VLM's capabilities. Second, we rigorously investigate VLMs along key design axes, including pretrained visual representations and quantifying the tradeoffs of using base vs. instruct-tuned language models, amongst others. We couple our analysis with three resource contributions: (1) a unified framework for evaluating VLMs, (2) optimized, flexible code for VLM training, and (3) checkpoints for all models, including a family of VLMs at the 7-13B scale that strictly outperform InstructBLIP and LLaVa v1.5, the state-of-the-art in open-source VLMs.

VLM이 쏟아지는 중에 정리를 하고 가자는 제안. 통합된 평가 슈트와 학습 프레임워크를 만든 다음 이미지 처리, 이미지 인코더 앙상블, LM 등에 대해 비교 분석을 했습니다.

#vision-language #framework #evaluation

Suggest that clean up environment around VLMs which vast amount of it occuring. Built unified evaluation suite and training framework, and did ablation studies on image processing, image encoder ensemble, and LM choices.