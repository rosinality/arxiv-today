https://publications.reka.ai/reka-vibe-eval.pdf

*Vibe-Eval: A hard evaluation suite for measuring progress of multimodal language models* (Piotr Padlewski, Max Bain, Matthew Henderson, Zhongkai Zhu, Nishant Relan, Hai Pham, Donovan Ong, Kaloyan Aleksiev, Aitor Ormazabal, Samuel Phua, Ethan Yeo, Eugenie Lamprecht, Qi Liu, Yuqi Wang, Eric Chen, Deyu Fu, Lei Li, Che Zheng, Cyprien de Masson d’Autume, Dani Yogatama, Mikel Artetxe, Yi Tay)

> We introduce Vibe-Eval: a new open benchmark and framework for evaluating multimodal chat models. Vibe-Eval consists of 269 visual understanding prompts, including 100 of hard difficulty, and complete with gold-standard responses authored by experts. Vibe-Eval is open-ended and challenging with dual objectives: (i) vibe checking multimodal chat models for day-to-day tasks and (ii) deeply challenging and probing the capabilities of present frontier models. To this end, our hard set contains > 50% questions that all frontier models answer incorrectly. We explore the nuances of designing, evaluating, and ranking models on ultra challenging prompts. We also discuss trade-offs between human and automatic evaluation, and show that automatic model evaluation using Reka Core roughly correlates to human judgment. We have made API access free-of-charge for the purpose of lightweight evaluation with the intention to run formal human evaluations for public models that do well on the Vibe-Eval automatic scores. We release the evaluation code and data at github.com/reka-ai/reka-vibe-eval.

Reka의 고난이도 Vision-Language 벤치마크. Inverse Scaling이 나타나는 샘플도 발견했네요.

모델 성능이 높아지면서 고난이도이면서 고품질이고 타당한 벤치마크에 대한 필요가 증가하고 있습니다. 그러나 이런 벤치마크를 만드는 것은 그만큼 더 까다롭겠죠. 요즘 흥미로운 사례인 GPQA에 대해서도 이런저런 말이 있더군요. (https://x.com/typedfemale/status/1783951432590188916)

#benchmark 