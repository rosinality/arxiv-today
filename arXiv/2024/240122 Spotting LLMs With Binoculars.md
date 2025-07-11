https://arxiv.org/abs/2401.12070

*Spotting LLMs With Binoculars: Zero-Shot Detection of Machine-Generated Text* (Abhimanyu Hans, Avi Schwarzschild, Valeriia Cherepanova, Hamid Kazemi, Aniruddha Saha, Micah Goldblum, Jonas Geiping, Tom Goldstein)

> Detecting text generated by modern large language models is thought to be hard, as both LLMs and humans can exhibit a wide range of complex behaviors. However, we find that a score based on contrasting two closely related language models is highly accurate at separating human-generated and machine-generated text. Based on this mechanism, we propose a novel LLM detector that only requires simple calculations using a pair of pre-trained LLMs. The method, called Binoculars, achieves state-of-the-art accuracy without any training data. It is capable of spotting machine text from a range of modern LLMs without any model-specific modifications. We comprehensively evaluate Binoculars on a number of text sources and in varied situations. Over a wide range of document types, Binoculars detects over 90% of generated samples from ChatGPT (and other LLMs) at a false positive rate of 0.01%, despite not being trained on any ChatGPT data.

LLM이 생성한 텍스트 검출. LLM이 생성한 텍스트는 LLM의 Perplexity가 낮을 것이기에 Perplexity를 쓸 수 있겠지만, 프롬프트가 없으면 LLM에게도 Perplexity가 높을 수 있습니다. 예를 들어 카피바라와 천체물리학자라는 주제로 생성한 텍스트는 프롬프트 없이 보면 Perplexity가 높겠죠.

그래서 모델 두 개를 준비해서 모델 사이의 Cross Entropy로 Normalize를 해줍니다. 모델 두 개 사이의 차이보다 사람의 텍스트의 차이가 클 것이라는 가정이죠. 표절 검출 같이 사용하기에는 1%의 에러율도 조심스럽지만 검출할 수 있다는 것 자체는 여러모로 유용할 수 있을 것 같네요.

#llm 