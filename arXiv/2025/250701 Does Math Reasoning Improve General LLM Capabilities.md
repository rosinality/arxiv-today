https://arxiv.org/abs/2507.00432

*Does Math Reasoning Improve General LLM Capabilities? Understanding Transferability of LLM Reasoning* (Maggie Huan, Yuetai Li, Tuney Zheng, Xiaoyu Xu, Seungone Kim, Minxin Du, Radha Poovendran, Graham Neubig, Xiang Yue)

> Math reasoning has become the poster child of progress in large language models (LLMs), with new models rapidly surpassing human-level performance on benchmarks like MATH and AIME. But as math leaderboards improve week by week, it is worth asking: do these gains reflect broader problem-solving ability or just narrow overfitting? To answer this question, we evaluate over 20 open-weight reasoning-tuned models across a broad suite of tasks, including math, scientific QA, agent planning, coding, and standard instruction-following. We surprisingly find that most models that succeed in math fail to transfer their gains to other domains. To rigorously study this phenomenon, we conduct controlled experiments on Qwen3-14B models using math-only data but different tuning methods. We find that reinforcement learning (RL)-tuned models generalize well across domains, while supervised fine-tuning (SFT)-tuned models often forget general capabilities. Latent-space representation and token-space distribution shift analyses reveal that SFT induces substantial representation and output drift, while RL preserves general-domain structure. Our results suggest a need to rethink standard post-training recipes, particularly the reliance on SFT-distilled data for advancing reasoning models.

수학에 대해 학습한 추론 모델이 다른 도메인에도 일반화가 되는가라는 질문. RL로 학습한 경우에는 되는데 SFT로 한 경우에는 안 된다고. RL을 하라던 사람들이 또다시 1승을 거두는군요.

<english>
Question of it is possible for model trained on math to generalize to the other domains. The result is RL allows, and SFT hinders. It is another one point for the people who always insists to adopt RL.
</english>

#generalization #rl #reasoning 