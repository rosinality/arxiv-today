https://arxiv.org/abs/2406.01940

*Process-Driven Autoformalization in Lean 4* (Jianqiao Lu, Zhengying Liu, Yingjia Wan, Yinya Huang, Haiming Wang, Zhicheng Yang, Jing Tang, Zhijiang Guo)

> Autoformalization, the conversion of natural language mathematics into formal languages, offers significant potential for advancing mathematical reasoning. However, existing efforts are limited to formal languages with substantial online corpora and struggle to keep pace with rapidly evolving languages like Lean 4. To bridge this gap, we propose a new benchmark \textbf{Form}alization for \textbf{L}ean~\textbf{4} (\textbf{\name}) designed to evaluate the autoformalization capabilities of large language models (LLMs). This benchmark encompasses a comprehensive assessment of questions, answers, formal statements, and proofs. Additionally, we introduce a \textbf{P}rocess-\textbf{S}upervised \textbf{V}erifier (\textbf{PSV}) model that leverages the precise feedback from Lean 4 compilers to enhance autoformalization. Our experiments demonstrate that the PSV method improves autoformalization, enabling higher accuracy using less filtered training data. Furthermore, when fine-tuned with data containing detailed process information, PSV can leverage the data more effectively, leading to more significant improvements in autoformalization for Lean 4. Our dataset and code are available at \url{https://github.com/rookie-joe/PDA}.

Lean을 타겟으로 한 Autoformalization 연구. 최근 나왔던 Lean을 사용한 증명 모델 구축의 첫 단계에 해당하는 부분이기도 합니다. (https://arxiv.org/abs/2405.14333)

Lean 컴파일러의 출력 결과를 사용해 Outcome/Process Supervision을 확보하는 방식이네요. 앞으로 LLM + 수학 연구를 하려면 Lean을 공부해야 하지 않을까 싶기도 합니다.

#math #rlaif #llm

# Links

[[240523 DeepSeek-Prover.md]]