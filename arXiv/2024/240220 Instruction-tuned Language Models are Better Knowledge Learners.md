https://arxiv.org/abs/2402.12847

*Instruction-tuned Language Models are Better Knowledge Learners* (Zhengbao Jiang, Zhiqing Sun, Weijia Shi, Pedro Rodriguez, Chunting Zhou, Graham Neubig, Xi Victoria Lin, Wen-tau Yih, Srinivasan Iyer)

> In order for large language model (LLM)-based assistants to effectively adapt to evolving information needs, it must be possible to update their factual knowledge through continued training on new data. The standard recipe for doing so involves continued pre-training on new documents followed by instruction-tuning on question-answer (QA) pairs. However, we find that LLMs trained with this recipe struggle to answer questions, even though the perplexity of documents is minimized. We found that QA pairs are generally straightforward, while documents are more complex, weaving many factual statements together in an intricate manner. Therefore, we hypothesize that it is beneficial to expose LLMs to QA pairs before continued pre-training on documents so that the process of encoding knowledge from complex documents takes into account how this knowledge is accessed through questions. Based on this, we propose pre-instruction-tuning (PIT), a method that instruction-tunes on questions prior to training on documents. This contrasts with standard instruction-tuning, which learns how to extract knowledge after training on documents. Extensive experiments and ablation studies demonstrate that PIT significantly enhances the ability of LLMs to absorb knowledge from new documents, outperforming standard instruction-tuning by 17.8%.

Instruction Tuning을 한 다음 문서를 학습시키는 것이 문서를 학습시킨 다음 Instruction Tuning을 하는 것보다 낫다는 결과. 학습 과정에서 문서를 인코딩하는 방식에 Instruction을 통해 정보를 사용하는 방식이 결부될 수 있다는 가정입니다.

Instruction Tuning 데이터를 프리트레이닝에 포함시키는 것이 유행인데 그것이 벤치마크 스코어 높이기 이상의 의미를 가질 수 있다는 증거일 수 있겠네요.

#instruction-tuning #pretraining 