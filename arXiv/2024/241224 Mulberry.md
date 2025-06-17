https://arxiv.org/abs/2412.18319

*Mulberry: Empowering MLLM with o1-like Reasoning and Reflection via Collective Monte Carlo Tree Search* (Huanjin Yao, Jiaxing Huang, Wenhao Wu, Jingyi Zhang, Yibo Wang, Shunyu Liu, Yingjie Wang, Yuxin Song, Haocheng Feng, Li Shen, Dacheng Tao)

> In this work, we aim to develop an MLLM that understands and solves questions by learning to create each intermediate step of the reasoning involved till the final answer. To this end, we propose Collective Monte Carlo Tree Search (CoMCTS), a new learning-to-reason method for MLLMs, which introduces the concept of collective learning into ``tree search'' for effective and efficient reasoning-path searching and learning. The core idea of CoMCTS is to leverage collective knowledge from multiple models to collaboratively conjecture, search and identify effective reasoning paths toward correct answers via four iterative operations including Expansion, Simulation and Error Positioning, Backpropagation, and Selection. Using CoMCTS, we construct Mulberry-260k, a multimodal dataset with a tree of rich, explicit and well-defined reasoning nodes for each question. With Mulberry-260k, we perform collective SFT to train our model, Mulberry, a series of MLLMs with o1-like step-by-step Reasoning and Reflection capabilities. Extensive experiments demonstrate the superiority of our proposed methods on various benchmarks. Code will be available at https://github.com/HJYao00/Mulberry

Vision-Language 모델에 대한 추론 능력 주입. 여러 개의 MLLM을 사용해 추론 경로를 생성하는 MCTS 기반이군요. 경로를 평가하는 것 또한 여러 MLLM을 프롬프팅해서 점수를 내는 방식으로 진행했네요.

o1에서 MCTS를 사용했는가도 논쟁이 되고 있죠. 그렇지만 사실 더 중요한 것은 어떻게 Reward를 부여했는가일 것이라고 생각합니다.

<english>
Injecting reasoning ability for vision-language models. The method is based on MCTS using multiple MLLMs for generating reasoning traces. Evaluation of trajectory is also based on scoring by multiple MLLMs with prompts.

There is debate whether o1 has used MCTS. But I think how it assigned reward is more important thing.
</english>

#vision-language #multimodal #mcts #search #reasoning 