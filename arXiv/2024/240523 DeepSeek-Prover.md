https://arxiv.org/abs/2405.14333

*DeepSeek-Prover: Advancing Theorem Proving in LLMs through Large-Scale Synthetic Data* (Huajian Xin, Daya Guo, Zhihong Shao, Zhizhou Ren, Qihao Zhu, Bo Liu, Chong Ruan, Wenda Li, Xiaodan Liang)

> Proof assistants like Lean have revolutionized mathematical proof verification, ensuring high accuracy and reliability. Although large language models (LLMs) show promise in mathematical reasoning, their advancement in formal theorem proving is hindered by a lack of training data. To address this issue, we introduce an approach to generate extensive Lean 4 proof data derived from high-school and undergraduate-level mathematical competition problems. This approach involves translating natural language problems into formal statements, filtering out low-quality statements, and generating proofs to create synthetic data. After fine-tuning the DeepSeekMath 7B model on this synthetic dataset, which comprises 8 million formal statements with proofs, our model achieved whole-proof generation accuracies of 46.3% with 64 samples and 52% cumulatively on the Lean 4 miniF2F test, surpassing the baseline GPT-4 at 23.0% with 64 samples and a tree search reinforcement learning method at 41.0%. Additionally, our model successfully proved 5 out of 148 problems in the Lean 4 Formalized International Mathematical Olympiad (FIMO) benchmark, while GPT-4 failed to prove any. These results demonstrate the potential of leveraging large-scale synthetic data to enhance theorem-proving capabilities in LLMs. Both the synthetic dataset and the model will be made available to facilitate further research in this promising field.

이야기만 나오던 Lean 같은 Proof Assistant와 LLM을 결합한 증명 탐색과 데이터 생성, 학습 방법의 구체적인 사례가 등장했군요. 웹 데이터를 Formal Statement로 변환한 다음 증명을 탐색하고 그 결과를 통해 학습시키는 방법입니다.

7B 모델로 실험했는데 더 강력한 모델을 사용한다면 어디까지 도달할 수 있을지 궁금해지네요. DeepSeek의 연구들은 늘 인상적입니다.

#synthetic-data #search 