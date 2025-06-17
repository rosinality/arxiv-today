https://arxiv.org/abs/2410.02108

*ReGenesis: LLMs can Grow into Reasoning Generalists via Self-Improvement* (Xiangyu Peng, Congying Xia, Xinyi Yang, Caiming Xiong, Chien-Sheng Wu, Chen Xing)

> Post-training Large Language Models (LLMs) with explicit reasoning trajectories can enhance their reasoning abilities. However, acquiring such high-quality trajectory data typically demands meticulous supervision from humans or superior models, which can be either expensive or license-constrained. In this paper, we explore how far an LLM can improve its reasoning by self-synthesizing reasoning paths as training data without any additional supervision. Existing self-synthesizing methods, such as STaR, suffer from poor generalization to out-of-domain (OOD) reasoning tasks. We hypothesize it is due to that their self-synthesized reasoning paths are too task-specific, lacking general task-agnostic reasoning guidance. To address this, we propose Reasoning Generalist via Self-Improvement (ReGenesis), a method to self-synthesize reasoning paths as post-training data by progressing from abstract to concrete. More specifically, ReGenesis self-synthesizes reasoning paths by converting general reasoning guidelines into task-specific ones, generating reasoning structures, and subsequently transforming these structures into reasoning paths, without the need for human-designed task-specific examples used in existing methods. We show that ReGenesis achieves superior performance on all in-domain and OOD settings tested compared to existing methods. For six OOD tasks specifically, while previous methods exhibited an average performance decrease of approximately 4.6% after post training, ReGenesis delivers around 6.1% performance improvement. We also conduct in-depth analysis of our framework and show ReGenesis is effective across various LLMs and design choices.

추론에 대해 학습시키면 특정 과제에 특화된 추론 패턴을 학습해서 일반화가 어려워진다는 착상. 일반적인 추론 전략을 가져와서 구체적인 과제에 맞는 전략으로 수정하고, 이 전략에 따라 추론의 얼개를 작성한 다음 실제 추론을 생성하는 방법. 일반적인 추론 전략을 설정한다는 것은 Self-Discover와 (https://arxiv.org/abs/2402.03620) 비슷하네요.

<english>
The main idea is that if you train model to do reasoning it learns task-specific reasoning patterns that not be able to generalized. So it takes general reasoning strategies and modify it for specific tasks, and make a detailed strategies for reasoning, and write actual reasoning steps. It is similar to Self-Discover (https://arxiv.org/abs/2402.03620) in the aspect of utilizing general reasoning strategies.
</english>

#reasoning

# Links

[[240206 Self-Discover.md]]