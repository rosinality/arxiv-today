https://github.com/MiniMax-AI/MiniMax-M1/blob/main/MiniMax_M1_tech_report.pdf

*MiniMax-M1: Scaling Test-Time Compute Efficiently with Lightning Attention* (MiniMax)

> We introduce MiniMax-M1, the world’s first open-weight, large-scale hybrid-attention reasoning model. MiniMax-M1 is powered by a hybrid Mixture-of-Experts (MoE) architecture combined with a lightning attention mechanism. The model is developed based on our previous MiniMax-Text-01 model (MiniMax et al., 2025), which contains a total of 456 billion parameters with 45.9 billion parameters activated per token. The M1 model natively supports a context length of 1 million tokens, 8x the context size of DeepSeek R1. Furthermore, the lightning attention mechanism in MiniMax-M1 enables efficient scaling of test-time compute – For example, compared to DeepSeek R1, M1 consumes 25% of the FLOPs at a generation length of 100K tokens. These properties make M1 particularly suitable for complex tasks that require processing long inputs and thinking extensively. MiniMax-M1 is trained using large-scale reinforcement learning (RL) on diverse problems ranging from traditional mathematical reasoning to sandbox-based, real-world software engineering environments. In addition to the inherent efficiency advantage of lightning attention for RL training, we propose CISPO, a novel RL algorithm to further enhance RL efficiency. CISPO clips importance sampling weights rather than token updates, outperforming other competitive RL variants. Combining hybrid-attention and CISPO enables MiniMax- M1’s full RL training on 512 H800 GPUs to complete in only three weeks, with a rental cost of just $534,700. We release two versions of MiniMax-M1 models with 40K and 80K thinking budgets respectively, where the 40K model represents an intermediate phase of the 80K training. Experiments on standard benchmarks show that our models are comparable or superior to strong open-weight models such as the original DeepSeek-R1 and Qwen3-235B, with particular strengths in complex software engineering, tool utilization, and long-context tasks. Through efficient scaling of test-time compute, MiniMax-M1 serves as a strong foundation for next-generation language model agents to reason and tackle real-world challenges. We publicly release MiniMax-M1 at https://github.com/MiniMax-AI/MiniMax-M1.

MiniMax의 추론 모델. 7.5T를 추가 학습해서 총 19T 정도를 학습했군요. 재미있게도 합성 데이터를 의도적으로 배제했다고 언급하고 있네요.

RL 알고리즘에서는 토큰 업데이트를 클리핑하는 것이 아니라 Importance Sampling 가중치를 클리핑하는 방법을 썼군요. 학습-추론 갭도 그렇고 하이브리드 모델에서 발생하는 난점이 조금 있는 것 같습니다.

<english>
MiniMax's reasoning model. With additional 7.5T training model is trained with about 19T. Interestingly, they intentionally excluded synthetic data.

For RL algorithms instead of clip token updates they clipped importance sampling weights. Along with training-inference gaps, it seems that there are some picky points that occurs in hybrid models.
</english>

#reasoning #rl 