https://arxiv.org/abs/2406.13542

*Self-play with Execution Feedback: Improving Instruction-following Capabilities of Large Language Models* (Guanting Dong, Keming Lu, Chengpeng Li, Tingyu Xia, Bowen Yu, Chang Zhou, Jingren Zhou)

> One core capability of large language models (LLMs) is to follow natural language instructions. However, the issue of automatically constructing high-quality training data to enhance the complex instruction-following abilities of LLMs without manual annotation remains unresolved. In this paper, we introduce AutoIF, the first scalable and reliable method for automatically generating instruction-following training data. AutoIF transforms the validation of instruction-following data quality into code verification, requiring LLMs to generate instructions, the corresponding code to check the correctness of the instruction responses, and unit test samples to verify the code's correctness. Then, execution feedback-based rejection sampling can generate data for Supervised Fine-Tuning (SFT) and Reinforcement Learning from Human Feedback (RLHF) training. AutoIF achieves significant improvements across three training algorithms, SFT, Offline DPO, and Online DPO, when applied to the top open-source LLMs, Qwen2 and LLaMA3, in self-alignment and strong-to-weak distillation settings. Our code is publicly available at https://github.com/QwenLM/AutoIF.

Instruction Following 능력을 모델이 자체 생성한 데이터로 향상시키기. 여기서는 IFEval이나 FollowBench 같은 코드로 검증 가능한 경우가 많은 사례를 대상으로 하긴 했습니다. Qwen 2에도 들어갔다고 하네요.

꽤 복잡한데 Seed Instruction을 만들고, Instruction을 LLM으로 증폭하고,답변을 검증하는 함수를 LLM으로 작성하고, Back Translation으로 이 함수를 다시 검수해서 Insturction에 대한 검증 함수 페어를 만듭니다.

그 다음 유저 쿼리를 이 Instruction과 결합한 Instruction을 만든 다음 Instruction에 문제가 없는지를 검증하고 응답을 검증 함수로 검수합니다. 이 피드백을 사용해 정렬을 진행하네요.

#instruction-tuning #alignment #synthetic-data a