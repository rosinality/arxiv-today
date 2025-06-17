https://arxiv.org/abs/2404.14963

*Achieving >97% on GSM8K: Deeply Understanding the Problems Makes LLMs Perfect Reasoners* (Qihuang Zhong, Kang Wang, Ziyang Xu, Juhua Liu, Liang Ding, Bo Du, Dacheng Tao)

> Chain of Thought prompting strategy has enhanced the performance of Large Language Models (LLMs) across various NLP tasks. However, it still has shortcomings when dealing with complex reasoning tasks, following~\citet{cot_wei}, including understanding errors, calculation errors and process errors (e.g. missing-step and hallucinations). Subsequently, Our in-depth analysis of various error types has found that deeply understanding the whole problem is critical in addressing complicated reasoning tasks. In this paper, we proposed a novel prompt strategy called Deeply Understanding the Problems (DUP) prompting, inspired by how humans solve complex reasoning problems, designed to enhance the comprehensive understanding of problems by LLMs. It consists of three stages: 1) extract the core question; 2) find out problem-solving information based on the core question; 3) generate and extract answers by LLMs. We evaluate the performance of DUP prompting on ten diverse reasoning datasets. Experimental results suggest that DUP prompting significantly outperforms Zero-Shot CoT ~\cite{kojima2022large} across all datasets. Notably, DUP achieves \textbf{state-of-the-art on SVAMP (90.4\% to 94.2\%) and GSM8K (94.6\% to 97.1\%).}

핵심 질문을 추출하고, 그 질문에 관련된 정보를 추출한 다음 CoT. 단순하고 재미있는 프롬프팅 전략 같네요.

#prompt 