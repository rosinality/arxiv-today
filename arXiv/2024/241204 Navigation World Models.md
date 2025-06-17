https://arxiv.org/abs/2412.03572

*Navigation World Models* (Amir Bar, Gaoyue Zhou, Danny Tran, Trevor Darrell, Yann LeCun)

> Navigation is a fundamental skill of agents with visual-motor capabilities. We introduce a Navigation World Model (NWM), a controllable video generation model that predicts future visual observations based on past observations and navigation actions. To capture complex environment dynamics, NWM employs a Conditional Diffusion Transformer (CDiT), trained on a diverse collection of egocentric videos of both human and robotic agents, and scaled up to 1 billion parameters. In familiar environments, NWM can plan navigation trajectories by simulating them and evaluating whether they achieve the desired goal. Unlike supervised navigation policies with fixed behavior, NWM can dynamically incorporate constraints during planning. Experiments demonstrate its effectiveness in planning trajectories from scratch or by ranking trajectories sampled from an external policy. Furthermore, NWM leverages its learned visual priors to imagine trajectories in unfamiliar environments from a single input image, making it a flexible and powerful tool for next-generation navigation systems.

구글에 더해 (https://deepmind.google/discover/blog/genie-2-a-large-scale-foundation-world-model/) 메타에서도 액션을 입력으로 받는 이미지 생성 모델을 만들었군요. 상호작용이 가능해야 World Model이라고 할 수 있겠죠.

<english>
In addition to Google (https://deepmind.google/discover/blog/genie-2-a-large-scale-foundation-world-model/) Meta also developed image generation models that allows action as an input. Model could be world models only when it allow interaction.
</english>

#world-models 