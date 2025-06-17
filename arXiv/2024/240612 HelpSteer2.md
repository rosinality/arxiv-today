https://arxiv.org/abs/2406.08673

*HelpSteer2: Open-source dataset for training top-performing reward models* (Zhilin Wang, Yi Dong, Olivier Delalleau, Jiaqi Zeng, Gerald Shen, Daniel Egert, Jimmy J. Zhang, Makesh Narsimhan Sreedhar, Oleksii Kuchaiev)

> High-quality preference datasets are essential for training reward models that can effectively guide large language models (LLMs) in generating high-quality responses aligned with human preferences. As LLMs become stronger and better aligned, permissively licensed preference datasets, such as Open Assistant, HH-RLHF, and HelpSteer need to be updated to remain effective for reward modeling. Methods that distil preference data from proprietary LLMs such as GPT-4 have restrictions on commercial usage imposed by model providers. To improve upon both generated responses and attribute labeling quality, we release HelpSteer2, a permissively licensed preference dataset (CC-BY-4.0). Using a powerful internal base model trained on HelpSteer2, we are able to achieve the SOTA score (92.0%) on Reward-Bench's primary dataset, outperforming currently listed open and proprietary models, as of June 12th, 2024. Notably, HelpSteer2 consists of only ten thousand response pairs, an order of magnitude fewer than existing preference datasets (e.g., HH-RLHF), which makes it highly efficient for training reward models. Our extensive experiments demonstrate that reward models trained with HelpSteer2 are effective in aligning LLMs. In particular, we propose SteerLM 2.0, a model alignment approach that can effectively make use of the rich multi-attribute score predicted by our reward models. HelpSteer2 is available at https://huggingface.co/datasets/nvidia/HelpSteer2 and code is available at https://github.com/NVIDIA/NeMo-Aligner

NVIDIA도 꾸준히 LLM을 만들고 튜닝하고 있군요. 15B 레시피로 (https://arxiv.org/abs/2402.16819) 340B 모델도 만들었고 연구하던 방식을 따라 (https://arxiv.org/abs/2311.09528) 데이터셋 구축도 했습니다.

최근 어노테이션을 직접 하고 있는 쪽에서는 샘플 하나를 한 명이 어노테이션하는 것을 넘어 여러 명이 참여하는 방식으로 바꿨으리라고 생각하고 있었는데 여기에서도 최소 세 명이 어노테이션을 했다고 하는군요.

#alignment

# Links

[[231116 HelpSteer.md]]
[[240226 Nemotron-4 15B Technical Report.md]]