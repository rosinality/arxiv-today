https://arxiv.org/abs/2402.12366

*A Critical Evaluation of AI Feedback for Aligning Large Language Models* (Archit Sharma, Sedrick Keh, Eric Mitchell, Chelsea Finn, Kushal Arora, Thomas Kollar)

> Reinforcement learning with AI feedback (RLAIF) is a popular paradigm for improving the instruction-following abilities of powerful pre-trained language models. RLAIF first performs supervised fine-tuning (SFT) using demonstrations from a teacher model and then further fine-tunes the model with reinforcement learning (RL), using feedback from a critic model. While recent popular open-source models have demonstrated substantial improvements in performance from the RL step, in this paper we question whether the complexity of this RL step is truly warranted for AI feedback. We show that the improvements of the RL step are virtually entirely due to the widespread practice of using a weaker teacher model (e.g. GPT-3.5) for SFT data collection than the critic (e.g., GPT-4) used for AI feedback generation. Specifically, we show that simple supervised fine-tuning with GPT-4 as the teacher outperforms existing RLAIF pipelines. More generally, we find that the gains from RLAIF vary substantially across base model families, test-time evaluation protocols, and critic models. Finally, we provide a mechanistic explanation for when SFT may outperform the full two-step RLAIF pipeline as well as suggestions for making RLAIF maximally useful in practice.

GPT-4로 Preference Feedback을 주는 것의 효과는 SFT 과정에서 3.5 데이터를 썼기 때문이 아닐까 하는 분석. Preference Feedback을 주는 대신 GPT-4의 샘플로 SFT를 하면 성능이 비슷하더라는 결과입니다.

논의 부분에서 RLHF가 성공적인 것은 사람을 통한 SFT 데이터셋과 Preference 데이터셋의 구축 난이도의 차이 때문이고 GPT-4로 생성한 샘플을 쓴다면 비용적으로는 오히려 Preference 데이터가 비싸니 Preference 데이터를 사용하는 튜닝은 불필요한 것이 아닐까...하는 이야기를 하고 있네요.

전 그런 의미에서 RLHF에 집중하거나 혹은 RLHF된 모델의 샘플을 사용하는 것이 아닌 프리트레이닝된 LM에서 시작하는 RLAIF 방향의 탐색이 흥미로운 길이 아닌가 하는 생각이 있습니다. 물론 UltraFeedback처럼 GPT-4로 Preference 데이터를 더 잘 추출한다면 성능 개선이 있을 수 있겠지만요.

#rlhf #rlaif 