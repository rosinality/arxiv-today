https://arxiv.org/abs/2405.03553

*AlphaMath Almost Zero: process Supervision without process* (Guoxin Chen, Minpeng Liao, Chengxi Li, Kai Fan)

> Recent advancements in large language models (LLMs) have substantially enhanced their mathematical reasoning abilities. However, these models still struggle with complex problems that require multiple reasoning steps, frequently leading to logical or numerical errors. While numerical mistakes can largely be addressed by integrating a code interpreter, identifying logical errors within intermediate steps is more challenging. Moreover, manually annotating these steps for training is not only expensive but also demands specialized expertise. In this study, we introduce an innovative approach that eliminates the need for manual annotation by leveraging the Monte Carlo Tree Search (MCTS) framework to generate both the process supervision and evaluation signals automatically. Essentially, when a LLM is well pre-trained, only the mathematical questions and their final answers are required to generate our training data, without requiring the solutions. We proceed to train a step-level value model designed to improve the LLM's inference process in mathematical domains. Our experiments indicate that using automatically generated solutions by LLMs enhanced with MCTS significantly improves the model's proficiency in dealing with intricate mathematical reasoning tasks.

답을 사용한 Process Supervision 하나 더. 요즘 이 문제에 MCTS를 적용한 사례가 많이 등장하고 있군요. (https://arxiv.org/abs/2404.12253, https://arxiv.org/pdf/2405.00451) 사실상 방법은 수렴하고 있고 대규모로 질문과 답 페어를 확보할 수 있는 방법을 고안하는 것이 문제일지도 모르겠습니다.

#search

# Links

