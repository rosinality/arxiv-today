https://arxiv.org/abs/2503.23829

*Expanding RL with Verifiable Rewards Across Diverse Domains* (Yi Su, Dian Yu, Linfeng Song, Juntao Li, Haitao Mi, Zhaopeng Tu, Min Zhang, Dong Yu)

> Reinforcement learning (RL) with verifiable rewards (RLVR) has shown promising results in mathematical reasoning and coding tasks where well-structured reference answers are available. However, its applicability to broader domains remains underexplored. In this work, we study the extension of RLVR to more diverse domains such as medicine, chemistry, psychology, and economics. We observe high agreement in binary judgments across different large language models (LLMs) when objective reference answers exist, which challenges the necessity of large-scale annotation for training domain-specific reward models. To address the limitations of binary rewards when handling unstructured reference answers, we further incorporate model-based soft scoring into RLVR to improve its flexibility. Our experiments show that a distilled generative reward model can serve as an effective cross-domain verifier, providing reliable reward signals for RL without requiring domain-specific annotations. By fine-tuning a base 7B model using various RL algorithms against our reward model, we obtain policies that outperform state-of-the-art open-source aligned LLMs such as Qwen2.5-72B-Instruct and DeepSeek-R1-Distill-Qwen-32B by a large margin, across domains in free-form answer settings. This also strengthens RLVR's robustness and scalability, highlighting its potential for real-world applications with noisy or weak labels.

다양한 도메인에 대한 비구조화된 응답을 정답을 사용하는 Reward Model로 평가. DeepSeek-R1에서도 비슷한 방법을 언급하고 있죠. 여기에서 추론까지 사용하는 것을 생각할 수 있겠죠.

<english>
Evaluating unstructured responses from diverse domains using reward model which utilizes ground truth. DeepSeek-R1 mentioned similar approaches. We can also think employing reasoning for this.
</english>

#reasoning #rl #reward-model 