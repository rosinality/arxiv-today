https://arxiv.org/abs/2309.17400

Directly Fine-Tuning Diffusion Models on Differentiable Rewards (Kevin Clark, Paul Vicol, Kevin Swersky, David J Fleet)

differentiable reward function을 사용해 rl 없이 바로 diffusion 모델을 학습시키는 방법. 샘플링 함수를 미분해야 하기 때문에 메모리 소모가 엄청난데 lora, gradient checkpointing을 사용하고, 거기에 더해 마지막 샘플링 스텝에서만 backward를 하는 것 + 노이즈를 사용해 추가 샘플을 만들어서 gradient variance를 줄이는 방법을 사용했습니다.

#ddpm #alignment 