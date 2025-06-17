https://arxiv.org/abs/2410.15115

*On Designing Effective RL Reward at Training Time for LLM Reasoning* (Jiaxuan Gao, Shusheng Xu, Wenjie Ye, Weilin Liu, Chuyi He, Wei Fu, Zhiyu Mei, Guangju Wang, Yi Wu)

> Reward models have been increasingly critical for improving the reasoning capability of LLMs. Existing research has shown that a well-trained reward model can substantially improve model performances at inference time via search. However, the potential of reward models during RL training time still remains largely under-explored. It is currently unclear whether these reward models can provide additional training signals to enhance the reasoning capabilities of LLMs in RL training that uses sparse success rewards, which verify the correctness of solutions. In this work, we evaluate popular reward models for RL training, including the Outcome-supervised Reward Model (ORM) and the Process-supervised Reward Model (PRM), and train a collection of LLMs for math problems using RL by combining these learned rewards with success rewards. Surprisingly, even though these learned reward models have strong inference-time performances, they may NOT help or even hurt RL training, producing worse performances than LLMs trained with the success reward only. Our analysis reveals that an LLM can receive high rewards from some of these reward models by repeating correct but unnecessary reasoning steps, leading to a severe reward hacking issue. Therefore, we introduce two novel reward refinement techniques, including Clipping and Delta. The key idea is to ensure the accumulative reward of any reasoning trajectory is upper-bounded to keep a learned reward model effective without being exploited. We evaluate our techniques with multiple reward models over a set of 1.5B and 7B LLMs on MATH and GSM8K benchmarks and demonstrate that with a carefully designed reward function, RL training without any additional supervised tuning can improve all the evaluated LLMs, including the state-of-the-art 7B LLM Qwen2.5-Math-7B-Instruct on MATH and GSM8K benchmarks.

Process Reward Model을 사용해서 RL을 진행했을 때 발생한 Reward Hacking 문제에 대한 경험. 문제 해결에 도움이 되지 않는 문장들을 채워넣는 패턴이 발생했다고 하네요. 대응 방법 중 하나는 생성한 문장에 의해 문제 해결에 진전이 발생하는지를 측정하는 것. Process Reward는 Advantage여야 한다는 주장이 떠오르는군요. (https://arxiv.org/abs/2410.08146)

<english>
Experience on reward hacking when did RL with process reward model. The pattern that generates meaningless sentences is learned. One method to cope with this is measure whether there are progress of problem solving by generated sentences. It reminds me an earlier argument that process reward should be advantage. (https://arxiv.org/abs/2410.08146)
</english>

#rl

# Links

[[241010 Rewarding Progress.md]]