https://arxiv.org/abs/2408.14837

*Diffusion Models Are Real-Time Game Engines* (Dani Valevski, Yaniv Leviathan, Moab Arar, Shlomi Fruchter)

> We present GameNGen, the first game engine powered entirely by a neural model that enables real-time interaction with a complex environment over long trajectories at high quality. GameNGen can interactively simulate the classic game DOOM at over 20 frames per second on a single TPU. Next frame prediction achieves a PSNR of 29.4, comparable to lossy JPEG compression. Human raters are only slightly better than random chance at distinguishing short clips of the game from clips of the simulation. GameNGen is trained in two phases: (1) an RL-agent learns to play the game and the training sessions are recorded, and (2) a diffusion model is trained to produce the next frame, conditioned on the sequence of past frames and actions. Conditioning augmentations enable stable auto-regressive generation over long trajectories.

https://gamengen.github.io/

이제 Diffusion에서 DOOM이 돌아가는군요. 게임을 하는 에이전트로 수집한 데이터로 Diffusion을 학습시키는 구조입니다.

#diffusion #rl 