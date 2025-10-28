https://arxiv.org/abs/2510.18840

*See the Text: From Tokenization to Visual Reading* (Ling Xing, Alex Jinpeng Wang, Rui Yan, Hongyu Qu, Zechao Li, Jinhui Tang)

> People see text. Humans read by recognizing words as visual objects, including their shapes, layouts, and patterns, before connecting them to meaning, which enables us to handle typos, distorted fonts, and various scripts effectively. Modern large language models (LLMs), however, rely on subword tokenization, fragmenting text into pieces from a fixed vocabulary. While effective for high-resource languages, this approach over-segments low-resource languages, yielding long, linguistically meaningless sequences and inflating computation. In this work, we challenge this entrenched paradigm and move toward a vision-centric alternative. Our method, SeeTok, renders text as images (visual-text) and leverages pretrained multimodal LLMs to interpret them, reusing strong OCR and text-vision alignment abilities learned from large-scale multimodal training. Across three different language tasks, SeeTok matches or surpasses subword tokenizers while requiring 4.43 times fewer tokens and reducing FLOPs by 70.5%, with additional gains in cross-lingual generalization, robustness to typographic noise, and linguistic hierarchy. SeeTok signals a shift from symbolic tokenization to human-like visual reading, and takes a step toward more natural and cognitively inspired language models.

토크나이저를 텍스트 렌더링으로 대체하려는 시도 하나 더. 대체 무슨 일이 벌어지고 있는 것인지?

One more attempt of replacing tokenizer with rendered texts. What's happening here?

#vision-language #tokenizer 