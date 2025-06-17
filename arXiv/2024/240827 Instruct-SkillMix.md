https://arxiv.org/abs/2408.14774

*Instruct-SkillMix: A Powerful Pipeline for LLM Instruction Tuning* (Simran Kaur, Simon Park, Anirudh Goyal, Sanjeev Arora)

> We introduce Instruct-SkillMix, an automated approach for creating diverse, high quality SFT data. The Instruct-SkillMix pipeline involves two stages, each leveraging an existing powerful LLM: (1) Skill extraction: uses the LLM to extract core "skills" for instruction-following, either from existing datasets, or by directly prompting the model; (2) Data generation: uses the powerful LLM to generate (instruction, response) data that exhibit a randomly chosen pair of these skills. Here, the use of random skill combinations promotes diversity and difficulty. Vanilla SFT (i.e., no PPO, DPO, or RL methods) on data generated from Instruct-SkillMix leads to strong gains on instruction following benchmarks such as AlpacaEval 2.0, MT-Bench, and WildBench. With just $4$K examples, LLaMA-3-8B-Base achieves 42.76% length-controlled win rate on AlpacaEval 2.0. To our knowledge, this achieves state-of-the-art performance among all models that have only undergone SFT (no RL methods) and competes with proprietary models such as Claude 3 Opus and LLaMA-3.1-405B-Instruct. Ablation studies also suggest plausible reasons for why creating open instruction-tuning datasets via naive crowd-sourcing has proved difficult. Introducing low quality answers ("shirkers") in $20\%$ of Instruct-SkillMix examples causes performance to plummet, sometimes catastrophically. The Instruct-SkillMix pipeline is flexible and is adaptable to other settings.

Skill 기반으로 평가하는 방법을 개발한 배경 위에서 (https://arxiv.org/abs/2310.17567) Skill을 섞어서 Instruction을 생성하는 방법을 고안했군요. Llama 3가 시사한 것처럼 프롬프트를 증폭하는 방법은 Alignment에서 필수적인 부분이 되긴 했네요.

#alignment #instruction-tuning

# Links

[[231026 Skill-Mix.md]]