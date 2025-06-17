https://arxiv.org/abs/2402.13013

*Code Needs Comments: Enhancing Code LLMs with Comment Augmentation* (Demin Song, Honglin Guo, Yunhua Zhou, Shuhao Xing, Yudong Wang, Zifan Song, Wenwei Zhang, Qipeng Guo, Hang Yan, Xipeng Qiu, Dahua Lin)

> The programming skill is one crucial ability for Large Language Models (LLMs), necessitating a deep understanding of programming languages (PLs) and their correlation with natural languages (NLs). We examine the impact of pre-training data on code-focused LLMs' performance by assessing the comment density as a measure of PL-NL alignment. Given the scarcity of code-comment aligned data in pre-training corpora, we introduce a novel data augmentation method that generates comments for existing code, coupled with a data filtering strategy that filters out code data poorly correlated with natural language. We conducted experiments on three code-focused LLMs and observed consistent improvements in performance on two widely-used programming skill benchmarks. Notably, the model trained on the augmented data outperformed both the model used for generating comments and the model further trained on the data without augmentation.

코드에 주석을 추가한 다음 이 데이터로 추가 학습을 시켜본다는 아이디어. 다만 샘플의 주석은 코드의 개별 라인에 대한 설명에 가까워 보이긴 합니다. 일종의 Instruction 데이터로 보이기도 하네요.

코드에 대해 좀 더 추상적인 레벨의 주석을 붙이는 방향이 재미있겠다는 생각도 듭니다.

#code #synthetic-data 