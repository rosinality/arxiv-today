https://arxiv.org/abs/2401.13313

*InstructDoc: A Dataset for Zero-Shot Generalization of Visual Document Understanding with Instructions* (Ryota Tanaka, Taichi Iki, Kyosuke Nishida, Kuniko Saito, Jun Suzuki)

> We study the problem of completing various visual document understanding (VDU) tasks, e.g., question answering and information extraction, on real-world documents through human-written instructions. To this end, we propose InstructDoc, the first large-scale collection of 30 publicly available VDU datasets, each with diverse instructions in a unified format, which covers a wide range of 12 tasks and includes open document types/formats. Furthermore, to enhance the generalization performance on VDU tasks, we design a new instruction-based document reading and understanding model, InstructDr, that connects document images, image encoders, and large language models (LLMs) through a trainable bridging module. Experiments demonstrate that InstructDr can effectively adapt to new VDU datasets, tasks, and domains via given instructions and outperforms existing multimodal LLMs and ChatGPT without specific training.

문서 관련 데이터셋들을 모아 정리해서 데이터셋을 구축했네요. OCR 결과를 입력으로 받는 모델을 만들어서 실험했습니다.

#dataset #ocr 