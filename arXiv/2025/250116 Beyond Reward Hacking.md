https://arxiv.org/abs/2501.09620

*Beyond Reward Hacking: Causal Rewards for Large Language Model Alignment* (Chaoqi Wang, Zhuokai Zhao, Yibo Jiang, Zhaorun Chen, Chen Zhu, Yuxin Chen, Jiayi Liu, Lizhu Zhang, Xiangjun Fan, Hao Ma, Sinong Wang)

> Recent advances in large language models (LLMs) have demonstrated significant progress in performing complex tasks. While Reinforcement Learning from Human Feedback (RLHF) has been effective in aligning LLMs with human preferences, it is susceptible to spurious correlations in reward modeling. Consequently, it often introduces biases-such as length bias, sycophancy, conceptual bias, and discrimination that hinder the model's ability to capture true causal relationships. To address this, we propose a novel causal reward modeling approach that integrates causal inference to mitigate these spurious correlations. Our method enforces counterfactual invariance, ensuring reward predictions remain consistent when irrelevant variables are altered. Through experiments on both synthetic and real-world datasets, we show that our approach mitigates various types of spurious correlations effectively, resulting in more reliable and fair alignment of LLMs with human preferences. As a drop-in enhancement to the existing RLHF workflow, our causal reward modeling provides a practical way to improve the trustworthiness and fairness of LLM finetuning.

길이 같은 변수에 의해서 Spurious Correlation이 Reward Model에 미치는 영향을 억제하려는 시도. 결과적으로 이 변수에 의해서 Reward Score의 분포가 변화하는 것을 억제하는 Regularization을 적용하는 형태입니다.

인과 추정의 문제가 늘 그렇듯 Confounding Factor들을 어떻게 파악할 것인가가 문제가 되죠. (https://arxiv.org/abs/2409.13156)

<english>
The study that tried to suppress the effect on reward model of spurious correlations from variables like length. Resulting method is applying regularization that suppresses distribution changes from theses variables.

Like common causal estimation problems the most important problem is how we can find and specify these confounding factors. (https://arxiv.org/abs/2409.13156)
</english>

#reward-model #alignment #rlhf

# Links

[[240920 RRM.md]]