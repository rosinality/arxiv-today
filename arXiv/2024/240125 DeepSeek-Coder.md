https://arxiv.org/abs/2401.14196

*DeepSeek-Coder: When the Large Language Model Meets Programming -- The Rise of Code Intelligence* (Daya Guo, Qihao Zhu, Dejian Yang, Zhenda Xie, Kai Dong, Wentao Zhang, Guanting Chen, Xiao Bi, Y. Wu, Y.K. Li, Fuli Luo, Yingfei Xiong, Wenfeng Liang)

> The rapid development of large language models has revolutionized code intelligence in software development. However, the predominance of closed-source models has restricted extensive research and development. To address this, we introduce the DeepSeek-Coder series, a range of open-source code models with sizes from 1.3B to 33B, trained from scratch on 2 trillion tokens. These models are pre-trained on a high-quality project-level code corpus and employ a fill-in-the-blank task with a 16K window to enhance code generation and infilling. Our extensive evaluations demonstrate that DeepSeek-Coder not only achieves state-of-the-art performance among open-source code models across multiple benchmarks but also surpasses existing closed-source models like Codex and GPT-3.5. Furthermore, DeepSeek-Coder models are under a permissive license that allows for both research and unrestricted commercial use.

DeepSeek Coder 리포트. 2T 학습한 모델이었군요.

DeepSeek Coder의 디테일에서 가장 흥미로운 부분은 코드 파일들 사이의 의존성을 고려했다는 것이 아닐까 싶습니다. 이 선택의 효과가 Cross File Code Completion에서 살짝 나오는데 약간의 향상으로 보입니다. 다만 해로울 이유는 없지 않을까 싶네요.

#code #llm #pretraining 