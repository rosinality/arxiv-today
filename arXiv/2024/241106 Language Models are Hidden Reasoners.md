https://arxiv.org/abs/2411.04282

*Language Models are Hidden Reasoners: Unlocking Latent Reasoning Capabilities via Self-Rewarding* (Haolin Chen, Yihao Feng, Zuxin Liu, Weiran Yao, Akshara Prabhakar, Shelby Heinecke, Ricky Ho, Phil Mui, Silvio Savarese, Caiming Xiong, Huan Wang)

> Large language models (LLMs) have shown impressive capabilities, but still struggle with complex reasoning tasks requiring multiple steps. While prompt-based methods like Chain-of-Thought (CoT) can improve LLM reasoning at inference time, optimizing reasoning capabilities during training remains challenging. We introduce LaTent Reasoning Optimization (LaTRO), a principled framework that formulates reasoning as sampling from a latent distribution and optimizes it via variational approaches. LaTRO enables LLMs to concurrently improve both their reasoning process and ability to evaluate reasoning quality, without requiring external feedback or reward models. We validate LaTRO through experiments on GSM8K and ARC-Challenge datasets using multiple model architectures. On GSM8K, LaTRO improves zero-shot accuracy by an average of 12.5% over base models and 9.6% over supervised fine-tuning across Phi-3.5-mini, Mistral-7B, and Llama-3.1-8B. Our findings suggest that pre-trained LLMs possess latent reasoning capabilities that can be unlocked and enhanced through our proposed optimization approach in a self-improvement manner. The code of LaTRO is available at https://github.com/SalesforceAIResearch/LaTRO.

CoT를 샘플링한 다음 CoT가 주어졌을 때 정답의 Likelihood 변화를 Reward로 사용해 RLOO을 진행. 정답 대신 Likelihood를 사용한다면 정답의 정확함을 체크하는 루틴을 작성하는 것을 피할 수 있다는 측면에서 유용할 수 있다고 봅니다.

<english>
Samples multiple CoTs, and do RLOO using likelihood of the answer given CoT as a rewards. If we use likelihood instead of accuracy then we can avoid to make a function for check accuracy of the answer, and this could be useful for informal answers.
</english>

#reasoning 