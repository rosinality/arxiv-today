https://arxiv.org/abs/2404.03622

*Visualization-of-Thought Elicits Spatial Reasoning in Large Language Models* (Wenshan Wu, Shaoguang Mao, Yadong Zhang, Yan Xia, Li Dong, Lei Cui, Furu Wei)

> Large language models (LLMs) have exhibited impressive performance in language comprehension and various reasoning tasks. However, their abilities in spatial reasoning, a crucial aspect of human cognition, remain relatively unexplored. Human possess a remarkable ability to create mental images of unseen objects and actions through a process known as \textbf{the Mind's Eye}, enabling the imagination of the unseen world. Inspired by this cognitive capacity, we propose Visualization-of-Thought (\textbf{VoT}) prompting. VoT aims to elicit spatial reasoning of LLMs by visualizing their reasoning traces, thereby guiding subsequent reasoning steps. We employed VoT for multi-hop spatial reasoning tasks, including natural language navigation, visual navigation, and visual tiling in 2D grid worlds. Experimental results demonstrated that VoT significantly enhances the spatial reasoning abilities of LLMs. Notably, VoT outperformed existing multimodal large language models (MLLMs) in these tasks. While VoT works surprisingly well on LLMs, the ability to generate \textit{mental images} to facilitate spatial reasoning resembles the mind's eye process, suggesting its potential viability in MLLMs.

공간적 추론 과제를 할 때 사고 과정과 그에 따른 결과를 Chain of Thought처럼 이미로 입력을 해주면 어떨까 하는 아이디어.

이미지 생성 능력을 가진 모델이라면 텍스트로 표현하기 어려운 사고 과정에 이미지 생성을 사용해서 추론하는데 도움을 받을 수 있을 것이라는 생각을 합니다. 다만 현재 이미지 생성 능력은 이런 형태의 추론에 도움을 받을 수 있는 형태는 아닐 것 같긴 하네요.

#prompt 