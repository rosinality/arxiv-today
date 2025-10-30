https://github.com/MoonshotAI/Kimi-Linear/blob/master/tech_report.pdf

*Kimi Linear: An Expressive, Efficient Attention Architecture* (Kimi Team)

> We introduce Kimi Linear, a hybrid linear attention architecture that, for the first time, outperforms full attention under fair comparisons across various scenarios—including short-context, long-context, and reinforcement learning (RL) scaling regimes. At its core lies Kimi Delta Attention (KDA), an expressive linear attention module that extends Gated DeltaNet [111] with a finer-grained gating mechanism, enabling more effective use of limited finite-state RNN memory. Our bespoke chunkwise algorithm achieves high hardware efficiency through a specialized variant of the Diagonal-Plus-Low- Rank (DPLR) transition matrices, which substantially reduces computation compared to the general DPLR formulation while remaining more consistent with the classical delta rule. We pretrain a Kimi Linear model with 3B activated parameters and 48B total parameters, based on a layerwise hybrid of KDA and Multi-Head Latent Attention (MLA). Our experiments show that with an identical training recipe, Kimi Linear outperforms full MLA with a sizeable margin across all evaluated tasks, while reducing KV cache usage by up to 75% and achieving up to 6× decoding throughput for a 1M context. These results demonstrate that Kimi Linear can be a drop-in replacement for full attention architectures with superior performance and efficiency, including tasks with longer input and output lengths. To support further research, we open-source the KDA kernel and vLLM implementations 1, and release the pre-trained and instruction-tuned model checkpoints. 

Gated DeltaNet + Fine grained gating. 

Gated DeltaNet + fine grained gating, and NoPE for global attention. Outperforms pure attention in reasoning. I think what is really interesting about SSM is it can actually be better than vanilla due to different inductive bias.

What made me worry about NoPE is it may lose the ability to localize in long contexts. KDA shows maybe it can compensate for the lack of RoPE in global attention.

Test time training is a nice framework to think about sequence models. One interesting way to contrast gated linear attention like Mamba vs DeltaNet is full-batch GD vs mini-batch GD. https://arxiv.org/abs/2407.04620, https://arxiv.org/abs/2501.12352

One more point - standard benchmarks **are** not enough to verify effectiveness of architectures, especially on reasoning tasks. We need to **be** very thorough on this.

#efficient-attention #state-space-model 