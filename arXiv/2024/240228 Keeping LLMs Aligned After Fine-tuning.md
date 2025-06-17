https://arxiv.org/abs/2402.18540

*Keeping LLMs Aligned After Fine-tuning: The Crucial Role of Prompt Templates* (Kaifeng Lyu, Haoyu Zhao, Xinran Gu, Dingli Yu, Anirudh Goyal, Sanjeev Arora)

> Public LLMs such as the Llama 2-Chat have driven huge activity in LLM research. These models underwent alignment training and were considered safe. Recently Qi et al. (2023) reported that even benign fine-tuning (e.g., on seemingly safe datasets) can give rise to unsafe behaviors in the models. The current paper is about methods and best practices to mitigate such loss of alignment. Through extensive experiments on several chat models (Meta's Llama 2-Chat, Mistral AI's Mistral 7B Instruct v0.2, and OpenAI's GPT-3.5 Turbo), this paper uncovers that the prompt templates used during fine-tuning and inference play a crucial role in preserving safety alignment, and proposes the "Pure Tuning, Safe Testing" (PTST) principle -- fine-tune models without a safety prompt, but include it at test time. Fine-tuning experiments on GSM8K, ChatDoctor, and OpenOrca show that PTST significantly reduces the rise of unsafe behaviors, and even almost eliminates them in some cases.

안전에 대해 정렬된 LM을 Helpfulness에 대해 파인튜닝하면 안전성이 깨지는 경향이 있는데 이에 대한 대응. 파인튜닝 할 때는 안전 관련 프롬프트가 없이 하고 추론할 때는 안전 프롬프트를 사용하면 된다고 합니다. 재미있네요.

#finetuning #prompt #safety 