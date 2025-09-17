https://arxiv.org/abs/2507.18391

*Revisiting LLM Reasoning via Information Bottleneck* (Shiye Lei, Zhihao Cheng, Kai Jia, Dacheng Tao)

> Large language models (LLMs) have recently demonstrated remarkable progress in reasoning capabilities through reinforcement learning with verifiable rewards (RLVR). By leveraging simple rule-based rewards, RL effectively incentivizes LLMs to produce extended chain-of-thought (CoT) reasoning trajectories, progressively guiding them toward correct answers. However, existing approaches remain largely heuristic and intuition-driven, limiting the development of principled methodologies. In this paper, we present a theoretical characterization of LLM reasoning grounded in information bottleneck (IB) principle, introducing IB-aware reasoning optimization (IBRO), a framework that encourages reasoning trajectories to be both informative about the final correct answer and generalizable across diverse prompts. We derive a practical token-level surrogate objective and propose an efficient approximation, resulting in the lightweight IB regularization method. This technique integrates seamlessly into existing RL-based post-training frameworks without additional computational overhead, requiring only a one-line code modification. Empirically, we validate IB regularization across multiple mathematical reasoning benchmarks and RL algorithms, demonstrating consistent improvements in LLM reasoning performance.

질문과 응답 사이에 추론을 Information Bottleneck으로 사용한다는 아이디어. 결과적으로는 엔트로피와 Advantage의 곱 형태라서 최근 엔트로피에 주목하는 연구들과 연결점이 있을지도?

The idea of using reasoning as an information bottleneck between instructions and answers. It takes the form of entropy multiplied by advantage, so it might have connections to recent research that emphasizes entropy?

#rl #reasoning 