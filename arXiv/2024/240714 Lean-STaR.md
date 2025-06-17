https://arxiv.org/abs/2407.10040

*Lean-STaR: Learning to Interleave Thinking and Proving* (Haohan Lin, Zhiqing Sun, Yiming Yang, Sean Welleck)

> Traditional language model-based theorem proving assumes that by training on a sufficient amount of formal proof data, a model will learn to prove theorems. Our key observation is that a wealth of informal information that is not present in formal proofs can be useful for learning to prove theorems. For instance, humans think through steps of a proof, but this thought process is not visible in the resulting code. We present Lean-STaR, a framework for training language models to produce informal thoughts prior to each step of a proof, thereby boosting the model's theorem-proving capabilities. Lean-STaR uses retrospective ground-truth tactics to generate synthetic thoughts for training the language model. At inference time, the trained model directly generates the thoughts prior to the prediction of the tactics in each proof step. Building on the self-taught reasoner framework, we then apply expert iteration to further fine-tune the model on the correct proofs it samples and verifies using the Lean solver. Lean-STaR achieves state-of-the-art results on the miniF2F-test benchmark within the Lean theorem proving environment, significantly outperforming base models (43.4% → 46.3%, Pass@64). We also analyze the impact of the augmented thoughts on various aspects of the theorem proving process, providing insights into their effectiveness.

Lean으로 증명을 하는 과정에서 형식 언어만 생성하는 것보다는 자연어로 생각하는 단계가 들어가면 좋지 않을까 하는 아이디어. 여기서 생각을 생성하는 것이 문제인데 생각을 바로 생성하는 것은 어렵지만 다음 증명 단계를 안다면 좀 더 할만하다는 아이디어입니다.

이 과정에서 더 강력한 모델(GPT-4)의 도움을 받긴 했습니다. 다만 이 과정 자체가 요즘 이야기가 나오는 행간을 생성하는 것과 관련이 있겠다 싶네요. 행간 생성과 자동화된 피드백이 좀 다른 아이디어이지만 같이 결합될 수 있겠다는 사례일 것 같습니다.

#math #prompt #search 