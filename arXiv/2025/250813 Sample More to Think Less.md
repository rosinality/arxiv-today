https://arxiv.org/abs/2508.09726

*Sample More to Think Less: Group Filtered Policy Optimization for Concise Reasoning* (Vaishnavi Shrivastava, Ahmed Awadallah, Vidhisha Balachandran, Shivam Garg, Harkirat Behl, Dimitris Papailiopoulos)

> Large language models trained with reinforcement learning with verifiable rewards tend to trade accuracy for length--inflating response lengths to achieve gains in accuracy. While longer answers may be warranted for harder problems, many tokens are merely "filler": repetitive, verbose text that makes no real progress. We introduce GFPO (Group Filtered Policy Optimization), which curbs this length explosion by sampling larger groups per problem during training and filtering responses to train on based on two key metrics: (1) response length and (2) token efficiency: reward per token ratio. By sampling more at training time, we teach models to think less at inference time. On the Phi-4-reasoning model, GFPO cuts GRPO's length inflation by 46-71% across challenging STEM and coding benchmarks (AIME 24/25, GPQA, Omni-MATH, LiveCodeBench) while maintaining accuracy. Optimizing for reward per token further increases reductions in length inflation to 71-85%. We also propose Adaptive Difficulty GFPO, which dynamically allocates more training resources to harder problems based on real-time difficulty estimates, improving the balance between computational efficiency and accuracy especially on difficult questions. GFPO demonstrates that increased training-time compute directly translates to reduced test-time compute--a simple yet effective trade-off for efficient reasoning.

샘플링 후 원하는 특성을 (응답 길이, 추론 효율성 등) 갖는 샘플만 사용해서 학습한다는 아이디어. 

Reasoning RL using top-k samples that have desired characteristics (such as response length and reasoning efficiency) choosen from the generations.

#rl #reasoning 