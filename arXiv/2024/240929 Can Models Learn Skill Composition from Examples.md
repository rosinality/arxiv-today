https://arxiv.org/abs/2409.19808

*Can Models Learn Skill Composition from Examples?* (Haoyu Zhao, Simran Kaur, Dingli Yu, Anirudh Goyal, Sanjeev Arora)

> As large language models (LLMs) become increasingly advanced, their ability to exhibit compositional generalization -- the capacity to combine learned skills in novel ways not encountered during training -- has garnered significant attention. This type of generalization, particularly in scenarios beyond training data, is also of great interest in the study of AI safety and alignment. A recent study introduced the SKILL-MIX evaluation, where models are tasked with composing a short paragraph demonstrating the use of a specified k-tuple of language skills. While small models struggled with composing even with k=3, larger models like GPT-4 performed reasonably well with k=5 and 6. In this paper, we employ a setup akin to SKILL-MIX to evaluate the capacity of smaller models to learn compositional generalization from examples. Utilizing a diverse set of language skills -- including rhetorical, literary, reasoning, theory of mind, and common sense -- GPT-4 was used to generate text samples that exhibit random subsets of k skills. Subsequent fine-tuning of 7B and 13B parameter models on these combined skill texts, for increasing values of k, revealed the following findings: (1) Training on combinations of k=2 and 3 skills results in noticeable improvements in the ability to compose texts with k=4 and 5 skills, despite models never having seen such examples during training. (2) When skill categories are split into training and held-out groups, models significantly improve at composing texts with held-out skills during testing despite having only seen training skills during fine-tuning, illustrating the efficacy of the training approach even with previously unseen skills. This study also suggests that incorporating skill-rich (potentially synthetic) text into training can substantially enhance the compositional capabilities of models.

Skill-Mix (https://arxiv.org/abs/2310.17567), 즉 필요한 능력의 수를 변화시켜 문제의 난이도를 조정하는 접근에 대해 모델을 이러한 문제에 대해 학습시켰을 때 성능이 어떻게 변화하는지를 분석한 연구.

주요한 발견은 1. 학습에서 사용하지 않은 능력들에 대해서도 일반화가 된다는 것 2. 학습에서 사용하지 않은 능력 조합의 숫자에 대해서도 일반화가 된다는 것입니다. 파인튜닝은 프리트레이닝된 모델에 잠재되어 있는 능력을 끌어낸다는 아이디어와 비슷하게 생각할 수 있을 듯 하네요. (여기서는 능력의 조합에 대한 Instruction Following 능력이 되겠죠.)

<english>
Based on Skill-Mix (https://arxiv.org/abs/2310.17567), a benchmark that which adjusts the difficulties of problem by changing number of required skills to solve, this study analyzes how performances are changed by training model on these problems.

Main findings is 1. Model generalizes to the skills that didn't used in training 2. Model generalizes the number of composed skills that aren't used in training. I think we can think this phenomena as the idea of finetuning is make capabilities of the model appear, that is already pretrained model has. (In this case it would be instruction following capabilities with respect to composition of skills.)
</english>

#generalization #llm

# Links

[[231026 Skill-Mix.md]]