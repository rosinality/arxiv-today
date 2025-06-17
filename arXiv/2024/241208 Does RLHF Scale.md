https://arxiv.org/abs/2412.06000

*Does RLHF Scale? Exploring the Impacts From Data, Model, and Method* (Zhenyu Hou, Pengfan Du, Yilin Niu, Zhengxiao Du, Aohan Zeng, Xiao Liu, Minlie Huang, Hongning Wang, Jie Tang, Yuxiao Dong)

> This study explores the scaling properties of Reinforcement Learning from Human Feedback (RLHF) in Large Language Models (LLMs). Although RLHF is considered an important step in post-training of LLMs, its scaling potential is still largely unknown. We systematically analyze key components in the RLHF framework--model size, data composition, and inference budget--and their impacts on performance. Our findings show that increasing data diversity and volume improves reward model performance, helping process-supervision models scale better. For policy training, more response samples per prompt boost performance initially but quickly plateau. And larger reward models offer modest gains in policy training. In addition, larger policy models benefit less from RLHF with a fixed reward model. Overall, RLHF scales less efficiently than pretraining, with diminishing returns from additional computational resources. Based on these observations, we propose strategies to optimize RLHF performance within computational limits.

프롬프트의 수, 프롬프트 당 샘플 수, Policy와 Reward 모델 크기에 따른 차이 등 RLHF의 Scaling에 대한 연구. 여기서도 Process Reward Model이 학습 도메인 외에 대해서는 잘 작동하지 않는다는 문제를 발견했네요.

<english>
Research on scaling of RLHF in aspect of the number of prompts, samples per prompt, difference from model size of policy and reward, and so on. This study also found process reward model does not work well outside of training domain.
</english>

#rlhf #reward-model 