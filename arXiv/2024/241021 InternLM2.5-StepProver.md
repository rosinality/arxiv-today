https://arxiv.org/abs/2410.15700

*InternLM2.5-StepProver: Advancing Automated Theorem Proving via Expert Iteration on Large-Scale LEAN Problems* (Zijian Wu, Suozhi Huang, Zhejian Zhou, Huaiyuan Ying, Jiayu Wang, Dahua Lin, Kai Chen)

> Large Language Models (LLMs) have emerged as powerful tools in mathematical theorem proving, particularly when utilizing formal languages such as LEAN. The major learning paradigm is expert iteration, which necessitates a pre-defined dataset comprising numerous mathematical problems. In this process, LLMs attempt to prove problems within the dataset and iteratively refine their capabilities through self-training on the proofs they discover. We propose to use large scale LEAN problem datasets Lean-workbook for expert iteration with more than 20,000 CPU days. During expert iteration, we found log-linear trends between solved problem amount with proof length and CPU usage. We train a critic model to select relatively easy problems for policy models to make trials and guide the model to search for deeper proofs. InternLM2.5-StepProver achieves open-source state-of-the-art on MiniF2F, Lean-Workbook-Plus, ProofNet, and Putnam benchmarks. Specifically, it achieves a pass of 65.9% on the MiniF2F-test and proves (or disproves) 17.0% of problems in Lean-Workbook-Plus which shows a significant improvement compared to only 9.5% of problems proved when Lean-Workbook-Plus was released. We open-source our models and searched proofs at https://github.com/InternLM/InternLM-Math and https://huggingface.co/datasets/internlm/Lean-Workbook.

Lean Workbook의 주장들을 기반으로 대규모 Expert Iteration을 진행해서 모델의 증명 능력 향상 시도를 했군요. CPU 시간으로 측정했을 때 1.5% 정도만이 실제로 유의미한 증명으로 이어졌고 98.5%는 결과로 이어지지 않았다고 하네요. 더 효율적인 탐색이 필요하다는 의미일 듯 합니다.

<english>
Tried to improve proving capabilities model by doing large scale expert iteration on Lean Workbook. Only 1.5% of CPU time was spent on actual meaning proving, and 98.5% of time was spent on non-results. So it suggest we need more efficient search methods.
</english>

#math #search 