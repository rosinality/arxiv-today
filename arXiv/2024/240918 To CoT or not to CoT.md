https://arxiv.org/abs/2409.12183

*To CoT or not to CoT? Chain-of-thought helps mainly on math and symbolic reasoning* (Zayne Sprague, Fangcong Yin, Juan Diego Rodriguez, Dongwei Jiang, Manya Wadhwa, Prasann Singhal, Xinyu Zhao, Xi Ye, Kyle Mahowald, Greg Durrett)

> Chain-of-thought (CoT) via prompting is the de facto method for eliciting reasoning capabilities from large language models (LLMs). But for what kinds of tasks is this extra ``thinking'' really helpful? To analyze this, we conducted a quantitative meta-analysis covering over 100 papers using CoT and ran our own evaluations of 20 datasets across 14 models. Our results show that CoT gives strong performance benefits primarily on tasks involving math or logic, with much smaller gains on other types of tasks. On MMLU, directly generating the answer without CoT leads to almost identical accuracy as CoT unless the question or model's response contains an equals sign, indicating symbolic operations and reasoning. Following this finding, we analyze the behavior of CoT on these problems by separating planning and execution and comparing against tool-augmented LLMs. Much of CoT's gain comes from improving symbolic execution, but it underperforms relative to using a symbolic solver. Our results indicate that CoT can be applied selectively, maintaining performance while saving inference costs. Furthermore, they suggest a need to move beyond prompt-based CoT to new paradigms that better leverage intermediate computation across the whole range of LLM applications.

Chain of Thought가 도움이 되는 경우는 수학이나 논리적 사고가 필요한 문제로 한정되는 것 같다는 연구. 그리고 이런 경우에는 Chain of Thought 대신 도구 사용으로 대체할 수 있는 경우도 많지 않은가 하는 주장이네요.

Quiet-STaR에서 (https://arxiv.org/abs/2403.09629) 지적한 것처럼 모든 토큰의 생성에 많은 추론 과정이 필요한 것은 아니겠죠. 비슷하게 생각할 수 있지 않을까 싶습니다.

#reasoning

# Links

[[240315 Pretraining with reading between-the-lines.md]]