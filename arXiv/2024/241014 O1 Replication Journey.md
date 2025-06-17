https://github.com/GAIR-NLP/O1-Journey

*O1 Replication Journey: A Strategic Progress Report - Part 1* (Yiwei Qin, Xuefeng Li, Haoyang Zou, Yixiu Liu, Shijie Xia, Zhen Huang, Yixin Ye, Weizhe Yuan, Zhengzhong Liu, Yuanzhi Li, Pengfei Liu)

> This paper introduces a pioneering approach to artificial intelligence research, embodied in our O1 Replication Journey. In response to the announcement of OpenAI’s groundbreaking O1 model, we embark on a transparent, real-time exploration to replicate its capabilities while reimagining the process of conducting and communicating AI research. Our methodology addresses critical challenges in modern AI research, including the insularity of prolonged team-based projects, delayed information sharing, and the lack of recognition for diverse contributions. By providing comprehensive, real-time documentation of our replication efforts, including both successes and failures, we aim to foster open science, accelerate collective advancement, and lay the groundwork for AI-driven scientific discovery. Our research progress report diverges significantly from traditional research papers, offering continuous updates, full process transparency, and active community engagement throughout the research journey. Technologically, we proposed the “journey learning” paradigm, which encourages models to learn not just shortcuts, but the complete exploration process, including trial and error, reflection, and backtracking. With only 327 training samples and without any additional tricks, journey learning outperformed conventional supervised learning by over 8% on the MATH dataset, demonstrating its extremely powerful potential. We believe this to be the most crucial component of O1 technology that we have successfully decoded. We share valuable resources including technical hypotheses and insights, cognitive exploration maps, custom-developed tools, etc at https://github.com/GAIR-NLP/O1-Journey

다들 o1을 어떻게 재현할 수 있을 것인가라는 문제에 뛰어들었군요. 여기서 생각한 방법은 Journey Learning이라고 이름 붙인, 정답으로 곧바로 이어지는 체인만이 아니라 오답이나 실수로 연결되는 체인들도 거쳐 정답으로 이어지는 체인을 통해 학습하는 방법이군요. Reward Model을 통해 추론 트리를 구성한 다음 이 트리에 대한 DFS로 체인을 만드는 방식입니다.

o1은 방법이 알려지지 않았기에 o1을 재현하자면 이 방법적인 측면에서 올바르게 접근해야 하고, 따라서 수많은 잠재적인 방법들 중 옳은 접근을 골라낼 좋은 판단력이 필요하겠죠.

<english>
Everyone jumped into how can we replicate o1. In this work authors thought the method that named as journey learning, which considers not only reasoning chains directly connected into the correct solution, but also chains connected into incorrect answers or mistakes to train the model. First construct reasoning tree with reward models and constructing chains using DFS on this tree.

o1 is the method we don't know how to replicate it. So we should follow correct approach to replicate it, and it requires good judgment to choose correct approach among vast amount of potential approaches.
</english>

#reasoning #search