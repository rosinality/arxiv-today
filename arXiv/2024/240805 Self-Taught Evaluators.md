https://arxiv.org/abs/2408.02666

*Self-Taught Evaluators* (Tianlu Wang, Ilia Kulikov, Olga Golovneva, Ping Yu, Weizhe Yuan, Jane Dwivedi-Yu, Richard Yuanzhe Pang, Maryam Fazel-Zarandi, Jason Weston, Xian Li)

> Model-based evaluation is at the heart of successful model development -- as a reward model for training, and as a replacement for human evaluation. To train such evaluators, the standard approach is to collect a large amount of human preference judgments over model responses, which is costly and the data becomes stale as models improve. In this work, we present an approach that aims to im-prove evaluators without human annotations, using synthetic training data only. Starting from unlabeled instructions, our iterative self-improvement scheme generates contrasting model outputs and trains an LLM-as-a-Judge to produce reasoning traces and final judgments, repeating this training at each new iteration using the improved predictions. Without any labeled preference data, our Self-Taught Evaluator can improve a strong LLM (Llama3-70B-Instruct) from 75.4 to 88.3 (88.7 with majority vote) on RewardBench. This outperforms commonly used LLM judges such as GPT-4 and matches the performance of the top-performing reward models trained with labeled examples.

LLM의 응답을 평가하는 Judge 모델을 만들기 위한 방법. Synthetic Pair를 만드는 것이 문제인데 이쪽에서는 프롬프트를 Rewriting해서 비슷하지만 약간 다른 프롬프트를 작성하게 하고 이 프롬프트에 대한 응답을 Weak Response로 설정했군요. 프롬프트가 약간 다르니 원 프롬프트에 대한 응답으로서는 부합하지 않는다는 아이디어죠.

Meta Rewarding과 비슷한 느낌이 드네요. (https://arxiv.org/abs/2407.19594)

#rlaif

# Links

[[240728 Meta-Rewarding Language Models.md]]