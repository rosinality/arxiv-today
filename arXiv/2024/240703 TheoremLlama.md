https://arxiv.org/abs/2407.03203

*TheoremLlama: Transforming General-Purpose LLMs into Lean4 Experts* (Ruida Wang, Jipeng Zhang, Yizhen Jia, Rui Pan, Shizhe Diao, Renjie Pi, Tong Zhang)

> Proving mathematical theorems using computer-verifiable formal languages like Lean significantly impacts mathematical reasoning. One approach to formal theorem proving involves generating complete proofs using Large Language Models (LLMs) based on Natural Language (NL) proofs. Similar methods have shown promising results in code generation. However, most modern LLMs exhibit suboptimal performance due to the scarcity of aligned NL and Formal Language (FL) theorem-proving data. This scarcity results in a paucity of methodologies for training LLMs and techniques to fully utilize their capabilities in composing formal proofs. To address the challenges, this paper proposes **TheoremLlama**, an end-to-end framework to train a general-purpose LLM to become a Lean4 expert. This framework encompasses NL-FL aligned dataset generation methods, training approaches for the LLM formal theorem prover, and techniques for LLM Lean4 proof writing. Using the dataset generation method, we provide *Open Bootstrapped Theorems* (OBT), an NL-FL aligned and bootstrapped dataset. A key innovation in this framework is the NL-FL bootstrapping method, where NL proofs are integrated into Lean4 code for training datasets, leveraging the NL reasoning ability of LLMs for formal reasoning. The **TheoremLlama** framework achieves cumulative accuracies of 36.48% and 33.61% on MiniF2F-Valid and Test datasets respectively, surpassing the GPT-4 baseline of 22.95% and 25.41%. We have also open-sourced our model checkpoints and generated dataset, and will soon make all the code publicly available.

요즘 유행하는 Lean 4를 사용한 수학 증명 능력 학습. Lean 4의 Mathlib4에 포함된 정의와 증명을 사용해 형식 언어를 자연어로 Deformalization을 하고 Lean 코드에 대한 설명을 자연어 주석으로 붙이도록 합니다.

이를 통해 Lean으로 증명을 작성하는 Instruction Tuning을 하고 샘플을 생성한 다음 Lean으로 검증한다는 흐름이군요.

Lean을 사용하는 연구는 결국 Formalization 문제가 가장 중요한 문제가 되고 있는 것 같긴 합니다. 수학자들이 참여하는 Formalization 작업이 수학계에 대해서나 AI에서나 의미가 있을 것 같다는 생각이 드네요. 물론 굉장히 어려운 작업이라고 하긴 합니다만.

#search #math 