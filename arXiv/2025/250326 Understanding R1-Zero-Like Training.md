https://arxiv.org/abs/2503.20783

*Understanding R1-Zero-Like Training: A Critical Perspective* (Zichen Liu, Changyu Chen, Wenjun Li, Penghui Qi, Tianyu Pang, Chao Du, Wee Sun Lee, Min Lin)

> DeepSeek-R1-Zero has shown that reinforcement learning (RL) at scale can directly enhance the reasoning capabilities of LLMs without supervised fine-tuning. In this work, we critically examine R1-Zero-like training by analyzing its two core components: base models and RL. We investigate a wide range of base models, including DeepSeek-V3-Base, to understand how pretraining characteristics influence RL performance. Our analysis reveals that DeepSeek-V3-Base already exhibit ''Aha moment'', while Qwen2.5 base models demonstrate strong reasoning capabilities even without prompt templates, suggesting potential pretraining biases. Additionally, we identify an optimization bias in Group Relative Policy Optimization (GRPO), which artificially increases response length (especially for incorrect outputs) during training. To address this, we introduce Dr. GRPO, an unbiased optimization method that improves token efficiency while maintaining reasoning performance. Leveraging these insights, we present a minimalist R1-Zero recipe that achieves 43.3% accuracy on AIME 2024 with a 7B base model, establishing a new state-of-the-art. Our code is available at https://github.com/sail-sg/understand-r1-zero.

GRPO에서 Length와 Reward Normalization을 빼버렸네요. Reward Normalization은 GRPO에서 특징적인 부분이었지만 Length로 평균하는 것은 RLHF에서도 대부분 채택한 방식이었죠. DAPO에서도 비슷한 지적을 했었죠. (https://arxiv.org/abs/2503.14476)

이렇게 수정하니 오답에서도 응답이 길어지는 현상이 제거됐네요. 이 현상에 대한 연구가 여러 건 나왔는데 말이죠.

<english>
The authors removed length and reward normalization from GRPO. Reward normalization was characteristic choice of GRPO, but length averaging was adopted in most implementations for RLHF. DAPO also pointed out similar issue (https://arxiv.org/abs/2503.14476).

After this modification the tendency of response length is increasing even for incorrect answers is removed. There was many researches dealt with this problem, but, anyway.
</english>

#rl #reasoning 