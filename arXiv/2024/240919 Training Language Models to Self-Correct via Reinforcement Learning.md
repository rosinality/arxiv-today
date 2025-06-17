https://arxiv.org/abs/2409.12917

*Training Language Models to Self-Correct via Reinforcement Learning* (Aviral Kumar, Vincent Zhuang, Rishabh Agarwal, Yi Su, John D Co-Reyes, Avi Singh, Kate Baumli, Shariq Iqbal, Colton Bishop, Rebecca Roelofs, Lei M Zhang, Kay McKinney, Disha Shrivastava, Cosmin Paduraru, George Tucker, Doina Precup, Feryal Behbahani, Aleksandra Faust)

> Self-correction is a highly desirable capability of large language models (LLMs), yet it has consistently been found to be largely ineffective in modern LLMs. Existing approaches for training self-correction either require multiple models or rely on a more capable model or other forms of supervision. To this end, we develop a multi-turn online reinforcement learning (RL) approach, SCoRe, that significantly improves an LLM's self-correction ability using entirely self-generated data. To build SCoRe, we first show that variants of supervised fine-tuning (SFT) on offline model-generated correction traces are insufficient for instilling self-correction behavior. In particular, we observe that training via SFT either suffers from a distribution mismatch between the training data and the model's own responses or implicitly prefers only a certain mode of correction behavior that is often not effective at test time. SCoRe addresses these challenges by training under the model's own distribution of self-generated correction traces and using appropriate regularization to steer the learning process into learning a self-correction strategy that is effective at test time as opposed to simply fitting high-reward responses for a given prompt. This regularization prescribes running a first phase of RL on a base model to generate a policy initialization that is less susceptible to collapse and then using a reward bonus to amplify self-correction during training. When applied to Gemini 1.0 Pro and 1.5 Flash models, we find that SCoRe achieves state-of-the-art self-correction performance, improving the base models' self-correction by 15.6% and 9.1% respectively on the MATH and HumanEval benchmarks.

아주 중요한 결과가 나왔네요. Self Correction을 어떻게 LLM이 하도록 할 수 있는지에 대한 방법입니다.

기본적으로는 SFT로는 안 된다는 것에서 시작합니다. 작은 수정만을 하는 경향이 있고 또한 Distribution Shift의 문제가 아주 크게 작용합니다.

그래서 답은 RL이죠.

SFT를 아예 빼버리고 1단계에서 첫 번째 응답 분포에 대한 KL Penalty를 건 상태에서 두 번째 응답에 대해 RL을 합니다. 2단계에서는 Self Correction을 촉진하도록 Reward Shaping을 한 다음 RL을 진행합니다.

이 문제를 RL로 다루는 것이 중요하다는 이야기는 이미 o1에 대해서도 나오고 있습니다. (https://x.com/wgussml/status/1834691198013129053) 따라서 이 문제에 대해 진지하다면 이 측면에서 생각해봐야겠죠.

#rl #reasoning 