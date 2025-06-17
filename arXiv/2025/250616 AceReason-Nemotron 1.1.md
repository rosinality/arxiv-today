https://arxiv.org/abs/2506.13284

*AceReason-Nemotron 1.1: Advancing Math and Code Reasoning through SFT and RL Synergy* (Zihan Liu, Zhuolin Yang, Yang Chen, Chankyu Lee, Mohammad Shoeybi, Bryan Catanzaro, Wei Ping)

> In this work, we investigate the synergy between supervised fine-tuning (SFT) and reinforcement learning (RL) in developing strong reasoning models. We begin by curating the SFT training data through two scaling strategies: increasing the number of collected prompts and the number of generated responses per prompt. Both approaches yield notable improvements in reasoning performance, with scaling the number of prompts resulting in more substantial gains. We then explore the following questions regarding the synergy between SFT and RL: (i) Does a stronger SFT model consistently lead to better final performance after large-scale RL training? (ii) How can we determine an appropriate sampling temperature during RL training to effectively balance exploration and exploitation for a given SFT initialization? Our findings suggest that (i) holds true, provided effective RL training is conducted, particularly when the sampling temperature is carefully chosen to maintain the temperature-adjusted entropy around 0.3, a setting that strikes a good balance between exploration and exploitation. Notably, the performance gap between initial SFT models narrows significantly throughout the RL process. Leveraging a strong SFT foundation and insights into the synergistic interplay between SFT and RL, our AceReason-Nemotron-1.1 7B model significantly outperforms AceReason-Nemotron-1.0 and achieves new state-of-the-art performance among Qwen2.5-7B-based reasoning models on challenging math and code benchmarks, thereby demonstrating the effectiveness of our post-training recipe. We release the model and data at: https://huggingface.co/nvidia/AceReason-Nemotron-1.1-7B

엔비디아의 추론 모델 실험. SFT를 많이 하면 성능이 향상된다, 그렇지만 RL 학습이 길어지면 그 차이는 감소한다, RL에서는 엔트로피를 적절하게 유지하는 것이 중요하다, RL을 통해 SFT로는 풀지 못하던 문제를 풀게 할 수 있다, 군요.

<english>
Experiment on reasoning model from NVIDIA. Main result is doing more SFT improves the performance, but performance gap decreases if RL training is prolonged, it is important to sustain adequate entropy for RL, and RL allows model to solve the problem that it was unable to solve using SFT.
</english>

#rl #reasoning 