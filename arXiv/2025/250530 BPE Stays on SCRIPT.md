https://arxiv.org/abs/2505.24689

*BPE Stays on SCRIPT: Structured Encoding for Robust Multilingual Pretokenization* (Sander Land, Catherine Arnett)

> Byte Pair Encoding (BPE) tokenizers, widely used in Large Language Models, face challenges in multilingual settings, including penalization of non-Western scripts and the creation of tokens with partial UTF-8 sequences. Pretokenization, often reliant on complex regular expressions, can also introduce fragility and unexpected edge cases. We propose SCRIPT (Script Category Representation in PreTokenization), a novel encoding scheme that bypasses UTF-8 byte conversion by using initial tokens based on Unicode script and category properties. This approach enables a simple, rule-based pretokenization strategy that respects script boundaries, offering a robust alternative to pretokenization strategies based on regular expressions. We also introduce and validate a constrained BPE merging strategy that enforces character integrity, applicable to both SCRIPT-BPE and byte-based BPE. Our experiments demonstrate that SCRIPT-BPE achieves competitive compression while eliminating encoding-based penalties for non-Latin-script languages.

유니코드의 카테고리 구조를 사용해서 Pretokenizer를 단순화한다는 아이디어네요.

<english>
The idea of simplify pretokenizer using category structure of unicode.
</english>

#tokenizer 