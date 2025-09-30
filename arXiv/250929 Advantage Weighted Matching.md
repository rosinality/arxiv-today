https://arxiv.org/abs/2509.25050

*Advantage Weighted Matching: Aligning RL with Pretraining in Diffusion Models* (Shuchen Xue, Chongjian Ge, Shilong Zhang, Yichen Li, Zhi-Ming Ma)

> Reinforcement Learning (RL) has emerged as a central paradigm for advancing Large Language Models (LLMs), where pre-training and RL post-training share the same log-likelihood formulation. In contrast, recent RL approaches for diffusion models, most notably Denoising Diffusion Policy Optimization (DDPO), optimize an objective different from the pretraining objectives--score/flow matching loss. In this work, we establish a novel theoretical analysis: DDPO is an implicit form of score/flow matching with noisy targets, which increases variance and slows convergence. Building on this analysis, we introduce \textbf{Advantage Weighted Matching (AWM)}, a policy-gradient method for diffusion. It uses the same score/flow-matching loss as pretraining to obtain a lower-variance objective and reweights each sample by its advantage. In effect, AWM raises the influence of high-reward samples and suppresses low-reward ones while keeping the modeling objective identical to pretraining. This unifies pretraining and RL conceptually and practically, is consistent with policy-gradient theory, reduces variance, and yields faster convergence. This simple yet effective design yields substantial benefits: on GenEval, OCR, and PickScore benchmarks, AWM delivers up to a $24\times$ speedup over Flow-GRPO (which builds on DDPO), when applied to Stable Diffusion 3.5 Medium and FLUX, without compromising generation quality. Code is available at https://github.com/scxue/advantage_weighted_matching.

Denoising Diffusion Policy Optimization이 노이즈 데이터에 대한 Denoising Score Matching과 동일하다는 것을 발견. 그리고 이는 깨끗한 데이터에 대한 Score Matching과 일치. 그렇다면 프리트레이닝 Objective와 같은 Score Matching을 사용하는 것이 낫지 않을까?

<english>
The authors found that Denoising Diffusion Policy Optimization is equivalent to Denoising Score Matching with noisy data, and this is also equivalent to Score Matching with clean data. Then wouldn't it better to use Score Matching for the post-train which is same with pretraining objective?
</english>

#diffusion #rl #post-training 