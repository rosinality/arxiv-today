https://arxiv.org/abs/2410.01490

*Extending Context Window of Large Language Models from a Distributional Perspective* (Yingsheng Wu. Yuxuan Gu, Xiaocheng Feng, Weihong Zhong, Dongliang Xu, Qing Yang, Hongtao Liu, Bing Qin)

> Scaling the rotary position embedding (RoPE) has become a common method for extending the context window of RoPE-based large language models (LLMs). However, existing scaling methods often rely on empirical approaches and lack a profound understanding of the internal distribution within RoPE, resulting in suboptimal performance in extending the context window length. In this paper, we propose to optimize the context window extending task from the view of rotary angle distribution. Specifically, we first estimate the distribution of the rotary angles within the model and analyze the extent to which length extension perturbs this distribution. Then, we present a novel extension strategy that minimizes the disturbance between rotary angle distributions to maintain consistency with the pre-training phase, enhancing the model's capability to generalize to longer sequences. Experimental results compared to the strong baseline methods demonstrate that our approach reduces by up to 72% of the distributional disturbance when extending LLaMA2's context window to 8k, and reduces by up to 32% when extending to 16k. On the LongBench-E benchmark, our method achieves an average improvement of up to 4.33% over existing state-of-the-art methods. Furthermore, Our method maintains the model's performance on the Hugging Face Open LLM benchmark after context window extension, with only an average performance fluctuation ranging from -0.12 to +0.22.

Context 확장 과정에서 RoPE의 각도 분포의 변화를 최소화하도록 Interpolation/Extrapolation 한다는 아이디어네요.

<english>
Idea of interpolate or extraploate to minimize disturbance of angle distribution of RoPE for context extension
</english>

#long-context #positional-encoding 