https://arxiv.org/abs/2504.06141

*Adversarial Training of Reward Models* (Alexander Bukharin, Haifeng Qian, Shengyang Sun, Adithya Renduchintala, Soumye Singhal, Zhilin Wang, Oleksii Kuchaiev, Olivier Delalleau, Tuo Zhao)

> Reward modeling has emerged as a promising approach for the scalable alignment of language models. However, contemporary reward models (RMs) often lack robustness, awarding high rewards to low-quality, out-of-distribution (OOD) samples. This can lead to reward hacking, where policies exploit unintended shortcuts to maximize rewards, undermining alignment. To address this challenge, we introduce Adv-RM, a novel adversarial training framework that automatically identifies adversarial examples -- responses that receive high rewards from the target RM but are OOD and of low quality. By leveraging reinforcement learning, Adv-RM trains a policy to generate adversarial examples that reliably expose vulnerabilities in large state-of-the-art reward models such as Nemotron 340B RM. Incorporating these adversarial examples into the reward training process improves the robustness of RMs, mitigating reward hacking and enhancing downstream performance in RLHF. We demonstrate that Adv-RM significantly outperforms conventional RM training, increasing stability and enabling more effective RLHF training in both synthetic and real-data settings.

Reward Model Ensemble로 추정한 Uncertainty에 대해 Adversarial Attack을 통해 Adversarial 샘플을 생성하는 모델을 학습. 그리고 이를 통해 Reward Model에 대한 Adversarial Training.

<english>
Training adversarial sample generator by doing adversarial attack on uncertainty measured by reward model ensembles. Then adversarial training on reward model is done using this.
</english>

#adversarial-training #reward-model 