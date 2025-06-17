https://arxiv.org/abs/2402.07896

*Suppressing Pink Elephants with Direct Principle Feedback* (Louis Castricato, Nathan Lile, Suraj Anand, Hailey Schoelkopf, Siddharth Verma, Stella Biderman)

> Existing methods for controlling language models, such as RLHF and Constitutional AI, involve determining which LLM behaviors are desirable and training them into a language model. However, in many cases, it is desirable for LLMs to be controllable \textit{at inference time}, so that they can be used in multiple contexts with diverse needs. We illustrate this with the \textbf{Pink Elephant Problem}: instructing an LLM to avoid discussing a certain entity (a ``Pink Elephant''), and instead discuss a preferred entity (``Grey Elephant''). We apply a novel simplification of Constitutional AI, \textbf{Direct Principle Feedback}, which skips the ranking of responses and uses DPO directly on critiques and revisions. Our results show that after DPF fine-tuning on our synthetic Pink Elephants dataset, our 13B fine-tuned LLaMA 2 model significantly outperforms Llama-2-13B-Chat and a prompted baseline, and performs as well as GPT-4 in on our curated test set assessing the Pink Elephant Problem.

코끼리는 생각하지 마, 즉 어떤 주제에 대해서 언급하지 말라는 금지 지시를 따르는 능력을 보완하려는 시도. 흥미로운 부분은 방법적으로 Constitutional AI의 RLAIF를 채택해서 생성된 응답에 대한 Critique와 Revision을 수행하는 형태로 접근했다는 것이네요. Constitutional AI에서 SFT와 Reward Modeling을 거친 것과는 다르게 여기서는 원 응답과 개선된 응답을 사용해 직접 DPO를 했습니다.

#alignment #rlaif 

This paper suggests a method for Pink Elephant problems, that is requiring model to do not mention specific topics. Interestingly authors used Constitutional AI style RLAIF methods, which critiques and revises original responses. Comparing to Constitutional AI, authors directly used revised and original responses as a pair for DPO, instead of doing SFT and reward modeling.