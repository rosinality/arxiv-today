https://arxiv.org/abs/2505.22660

*Maximizing Confidence Alone Improves Reasoning* (Mihir Prabhudesai, Lili Chen, Alex Ippoliti, Katerina Fragkiadaki, Hao Liu, Deepak Pathak)

> Reinforcement learning (RL) has enabled machine learning models to achieve significant advances in many fields. Most recently, RL has empowered frontier language models to solve challenging math, science, and coding problems. However, central to any RL algorithm is the reward function, and reward engineering is a notoriously difficult problem in any domain. In this paper, we propose RENT: Reinforcement Learning via Entropy Minimization -- a fully unsupervised RL method that requires no external reward or ground-truth answers, and instead uses the model's entropy of its underlying distribution as an intrinsic reward. We find that by reinforcing the chains of thought that yield high model confidence on its generated answers, the model improves its reasoning ability. In our experiments, we showcase these improvements on an extensive suite of commonly-used reasoning benchmarks, including GSM8K, MATH500, AMC, AIME, and GPQA, and models of varying sizes from the Qwen and Mistral families. The generality of our unsupervised learning method lends itself to applicability in a wide range of domains where external supervision is limited or unavailable.

엔트로피나 Majority Voting으로 정답 없이 추론 RL이 가능하다는 결과가 요즘 정말 많이 나오고 있죠 (https://arxiv.org/abs/2505.15134, https://arxiv.org/abs/2505.17454, https://arxiv.org/abs/2505.20347, https://arxiv.org/abs/2505.22453). 반대로 데이터를 사용해서 얻을 수 있는 것은 무엇인가를 묻는 것도 재미있지 않을까요.

<english>
There are so many results appearing it is possible to do reasoning RL without ground truth answers by using entropy or majority voting (https://arxiv.org/abs/2505.15134, https://arxiv.org/abs/2505.17454, https://arxiv.org/abs/2505.20347, https://arxiv.org/abs/2505.22453). Conversely, maybe it is interesting to ask what we can get by using the data.
</english>

#rl #reasoning 