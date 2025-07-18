https://arxiv.org/abs/2401.14953

*Learning Universal Predictors* (Jordi Grau-Moya, Tim Genewein, Marcus Hutter, Laurent Orseau, Grégoire Delétang, Elliot Catt, Anian Ruoss, Li Kevin Wenliang, Christopher Mattern, Matthew Aitchison, Joel Veness)

> Meta-learning has emerged as a powerful approach to train neural networks to learn new tasks quickly from limited data. Broad exposure to different tasks leads to versatile representations enabling general problem solving. But, what are the limits of meta-learning? In this work, we explore the potential of amortizing the most powerful universal predictor, namely Solomonoff Induction (SI), into neural networks via leveraging meta-learning to its limits. We use Universal Turing Machines (UTMs) to generate training data used to expose networks to a broad range of patterns. We provide theoretical analysis of the UTM data generation processes and meta-training protocols. We conduct comprehensive experiments with neural architectures (e.g. LSTMs, Transformers) and algorithmic data generators of varying complexity and universality. Our results suggest that UTM data is a valuable resource for meta-learning, and that it can be used to train neural networks capable of learning universal prediction strategies.

Universal Turing Machine에 랜덤 프로그램을 입력해 생성한 결과물로 모델을 학습시켰을 때 Solomonoff Induction을 근사할 수 있다는 연구. Solomonoff Induction이 무엇인지부터 문제인데 https://www.lesswrong.com/posts/Kyc5dFDzBg4WccrbK/an-intuitive-explanation-of-solomonoff-induction 이 글이 (길지만) 도움이 되는군요. 간단히 요약하면 데이터를 설명하는 가장 단순한 프로그램을 찾는 것이라고 할 수 있겠습니다.

이게 어떤 함의를 갖는 걸까요? 좀 생각해봐야할 문제일 것 같습니다. 한 가지 단서는 LLM과 Solomonoff Induction의 관계에 대한 추론이네요. LLM에서 In context Learning 능력이 발생한다는 것은 Solomonoff Induction을 근사하고 있다는 의미일 수 있고, Universal Turning Machine으로 생성된 데이터가 아니라 (사람이 풀기 원하는 과제들과 좀 더 잘 맞는) 사람의 텍스트 데이터로 학습된 것이라는 시각입니다.

#meta-learning

This paper suggests that by training models with outputs generated by universal turing machine, using random programs, can approximate solomonoff induction. Of course understanding of solomonoff induction is required to comprehend this. https://www.lesswrong.com/posts/Kyc5dFDzBg4WccrbK/an-intuitive-explanation-of-solomonoff-induction This article (slightly verbose) is helpful for that. Put it simply, it is problem of finding the simples program that explains a given data.

What could be the implication of this result? This raises intriguing questions. One hint is that reasoning about the relationship between LLMs and Solomonoff Induction in the paper. In-context learning capabilities of LLMs suggest that it approximiates solomonoff induction, and LLMs are just trained with text data produced by humans which is well-aligned to the problem we are want to solve, rather than the data generated by universal turing machine.