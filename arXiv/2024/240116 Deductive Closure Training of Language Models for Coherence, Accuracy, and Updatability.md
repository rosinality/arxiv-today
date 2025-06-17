https://arxiv.org/abs/2401.08574

*Deductive Closure Training of Language Models for Coherence, Accuracy, and Updatability* (Afra Feyza Akyürek, Ekin Akyürek, Leshem Choshen, Derry Wijaya, Jacob Andreas)

> While language models (LMs) can sometimes generate factually correct text and estimate truth values of individual claims, these generally do not reflect a globally coherent, manipulable model of the world. As a consequence, current LMs also generate incorrect or nonsensical content, and are difficult to edit and bring up to date. We present a method called Deductive Closure Training (DCT) that uses LMs themselves to identify implications of (and contradictions within) the text that they generate, yielding an efficient self-supervised procedure for improving LM factuality. Given a collection of seed documents, DCT prompts LMs to generate additional text implied by these documents, reason globally about the correctness of this generated text, and finally fine-tune on text inferred to be correct. Given seed documents from a trusted source, DCT provides a tool for supervised model updating; if seed documents are sampled from the LM itself, DCT enables fully unsupervised fine-tuning for improved coherence and accuracy. Across the CREAK, MQUaKE, and Reversal Curse datasets, supervised DCT improves LM fact verification and text generation accuracy by 3-26%; on CREAK fully unsupervised DCT improves verification accuracy by 12%. These results show that LMs' reasoning capabilities during inference can be leveraged during training to improve their reliability.

사실 관계 추론 능력을 향상시키기 위한 데이터를 구축하는 방법. 문서를 가져와서 그 문서를 기반으로 문서가 함의(Implication)하거나 혹은 모순(Contradiction)이 되는 문서들을 생성합니다. 그리고 이 문서들에 대한 LM의 확률과 논리적 일관성, 즉 모두 함의이거나 모순일 것이라는 기준으로 필터링 하는 방식이네요.

논리적 구조와 원본 문서라는 정보원을 통해 합성 데이터를 만들었다고 생각할 수 있지 않을까 싶네요. 합성 데이터에서 가장 흥미로운 부분은 어떻게 정보를 주입할 것인가이니까요.

#synthetic-data 