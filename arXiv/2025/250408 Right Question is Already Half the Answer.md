https://arxiv.org/abs/2504.05812

*Right Question is Already Half the Answer: Fully Unsupervised LLM Reasoning Incentivization* (Qingyang Zhang, Haitao Wu, Changqing Zhang, Peilin Zhao, Yatao Bian)

> While large language models (LLMs) have demonstrated exceptional capabilities in challenging tasks such as mathematical reasoning, existing methods to enhance reasoning ability predominantly rely on supervised fine-tuning (SFT) followed by reinforcement learning (RL) on reasoning-specific data after pre-training. However, these approaches critically depend on external supervisions--such as human labelled reasoning traces, verified golden answers, or pre-trained reward models--which limits scalability and practical applicability. In this work, we propose Entropy Minimized Policy Optimization (EMPO), which makes an early attempt at fully unsupervised LLM reasoning incentivization. EMPO does not require any supervised information for incentivizing reasoning capabilities (i.e., neither verifiable reasoning traces, problems with golden answers, nor additional pre-trained reward models). By continuously minimizing the predictive entropy of LLMs on unlabeled user queries in a latent semantic space, EMPO enables purely self-supervised evolution of reasoning capabilities with strong flexibility and practicality. Our experiments demonstrate competitive performance of EMPO on both mathematical reasoning and free-form commonsense reasoning tasks. Specifically, without any supervised signals, EMPO boosts the accuracy of Qwen2.5-Math-7B Base from 30.7\% to 48.1\% on mathematical benchmarks and improves truthfulness accuracy of Qwen2.5-7B Instruct from 87.16\% to 97.25\% on TruthfulQA.

최종 응답의 Semantic Entropy를 통해 추론 RL을 할 수 있다는 연구. Semantic Entropy는 불확실성 추정과 할루시네이션 탐지 목적으로 등장했었죠. (https://arxiv.org/abs/2302.09664, https://www.nature.com/articles/s41586-024-07421-0) 이건 정말로 프리트레이닝을 믿고 던지는 느낌이군요.

<english>
A study insists it is possible to do reasoning RL using semantic entropy of final answer. Semantic entropy is first suggested to do uncertainty estimation and detecting hallucinations (https://arxiv.org/abs/2302.09664, https://www.nature.com/articles/s41586-024-07421-0). This approach does reasoning training depending almost solely on pretraining.
</english>

#rl #reasoning #uncertainty 