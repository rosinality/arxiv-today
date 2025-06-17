https://arxiv.org/abs/2411.11694

*Technical Report: Enhancing LLM Reasoning with Reward-guided Tree Search* (Jinhao Jiang, Zhipeng Chen, Yingqian Min, Jie Chen, Xiaoxue Cheng, Jiapeng Wang, Yiru Tang, Haoxiang Sun, Jia Deng, Wayne Xin Zhao, Zheng Liu, Dong Yan, Jian Xie, Zhongyuan Wang, Ji-Rong Wen)

> Recently, test-time scaling has garnered significant attention from the research community, largely due to the substantial advancements of the o1 model released by OpenAI. By allocating more computational resources during the inference phase, large language models~(LLMs) can extensively explore the solution space by generating more thought tokens or diverse solutions, thereby producing more accurate responses. However, developing an o1-like reasoning approach is challenging, and researchers have been making various attempts to advance this open area of research. In this paper, we present a preliminary exploration into enhancing the reasoning abilities of LLMs through reward-guided tree search algorithms. This framework is implemented by integrating the policy model, reward model, and search algorithm. It is primarily constructed around a tree search algorithm, where the policy model navigates a dynamically expanding tree guided by a specially trained reward model. We thoroughly explore various design considerations necessary for implementing this framework and provide a detailed report of the technical aspects. To assess the effectiveness of our approach, we focus on mathematical reasoning tasks and conduct extensive evaluations on four challenging datasets, significantly enhancing the reasoning abilities of LLMs.

다들 추론 능력을 위해 노력하고 있죠. 여기서는 MCTS 기반이군요. Outcome Reward Model의 사용 등 다소 비전형적인 선택들이 있네요.

o1의 방법은 뭘까요? 지금 가장 중요한 문제인 듯 합니다.

<english>
Everybody pursuing reasoning now. This work based on MCTS. There are non-conventional choices like use of outcome reward models.

What is the method behind o1? It is currently most important problem.
</english>

#reasoning #search #mcts #reward-model 