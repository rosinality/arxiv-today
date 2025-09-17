https://arxiv.org/abs/2509.04394

*Transition Models: Rethinking the Generative Learning Objective* (Zidong Wang, Yiyuan Zhang, Xiaoyu Yue, Xiangyu Yue, Yangguang Li, Wanli Ouyang, Lei Bai)

> A fundamental dilemma in generative modeling persists: iterative diffusion models achieve outstanding fidelity, but at a significant computational cost, while efficient few-step alternatives are constrained by a hard quality ceiling. This conflict between generation steps and output quality arises from restrictive training objectives that focus exclusively on either infinitesimal dynamics (PF-ODEs) or direct endpoint prediction. We address this challenge by introducing an exact, continuous-time dynamics equation that analytically defines state transitions across any finite time interval. This leads to a novel generative paradigm, Transition Models (TiM), which adapt to arbitrary-step transitions, seamlessly traversing the generative trajectory from single leaps to fine-grained refinement with more steps. Despite having only 865M parameters, TiM achieves state-of-the-art performance, surpassing leading models such as SD3.5 (8B parameters) and FLUX.1 (12B parameters) across all evaluated step counts. Importantly, unlike previous few-step generators, TiM demonstrates monotonic quality improvement as the sampling budget increases. Additionally, when employing our native-resolution strategy, TiM delivers exceptional fidelity at resolutions up to 4096x4096.

임의의 두 시점에 대한 전환을 모델링하는 방법. 두 시점을 모델링하는 건 자주 시도되는 방법이 아닌가 싶음. (예를 들면 Inductive moment matching https://arxiv.org/abs/2503.07565).

Train a model to predict transitions between two timesteps. Modeling transitions between two arbitrary timesteps has often been tried in different ways, such as in Inductive Moment Matching (https://arxiv.org/abs/2503.07565).

#diffusion 