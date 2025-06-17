https://arxiv.org/abs/2506.03136

*Co-Evolving LLM Coder and Unit Tester via Reinforcement Learning* (Yinjie Wang, Ling Yang, Ye Tian, Ke Shen, Mengdi Wang)

> We propose CURE, a novel reinforcement learning framework with a dedicated reward design that co-evolves coding and unit test generation capabilities based on their interaction outcomes, without any ground-truth code as supervision. This approach enables flexible and scalable training and allows the unit tester to learn directly from the coder's mistakes. Our derived ReasonFlux-Coder-7B and 14B models improve code generation accuracy by 5.3% and Best-of-N accuracy by 9.0% after optimization on Qwen2.5-Instruct models, outperforming similarly sized Qwen-Coder, DeepSeek-Coder, and Seed-Coder. They naturally extend to downstream tasks such as test-time scaling and agentic coding-achieving a 8.1% improvement over the base model. For the long-CoT model, our ReasonFlux-Coder-4B consistently outperforms Qwen3-4B while achieving 64.8% inference efficiency in unit test generation. Notably, we also find that our model can serve as an effective reward model for reinforcement learning on base models. Project: https://github.com/Gen-Verse/CURE

코드 생성과 함께 유닛 테스트 생성을 학습. Verification을 같이 학습시키는 것처럼 (https://arxiv.org/abs/2505.13445, https://arxiv.org/abs/2506.01369) 하지 않을 이유가 딱히 없을 것 같네요.

<english>
Training unit test generation with code generation at the same time. Like training verification simulataneously (https://arxiv.org/abs/2505.13445, https://arxiv.org/abs/2506.01369) I think there are no reason to not to do that.
</english>

#rl #reasoning 