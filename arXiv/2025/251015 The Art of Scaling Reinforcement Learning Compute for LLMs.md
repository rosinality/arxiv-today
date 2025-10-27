https://arxiv.org/abs/2510.13786

*The Art of Scaling Reinforcement Learning Compute for LLMs* (Devvrit Khatri, Lovish Madaan, Rishabh Tiwari, Rachit Bansal, Sai Surya Duvvuri, Manzil Zaheer, Inderjit S. Dhillon, David Brandfonbrener, Rishabh Agarwal)

> Reinforcement learning (RL) has become central to training large language models (LLMs), yet the field lacks predictive scaling methodologies comparable to those established for pre-training. Despite rapidly rising compute budgets, there is no principled understanding of how to evaluate algorithmic improvements for scaling RL compute. We present the first large-scale systematic study, amounting to more than 400,000 GPU-hours, that defines a principled framework for analyzing and predicting RL scaling in LLMs. We fit sigmoidal compute-performance curves for RL training and ablate a wide range of common design choices to analyze their effects on asymptotic performance and compute efficiency. We observe: (1) Not all recipes yield similar asymptotic performance, (2) Details such as loss aggregation, normalization, curriculum, and off-policy algorithm primarily modulate compute efficiency without materially shifting the asymptote, and (3) Stable, scalable recipes follow predictable scaling trajectories, enabling extrapolation from smaller-scale runs. Combining these insights, we propose a best-practice recipe, ScaleRL, and demonstrate its effectiveness by successfully scaling and predicting validation performance on a single RL run scaled up to 100,000 GPU-hours. Our work provides both a scientific framework for analyzing scaling in RL and a practical recipe that brings RL training closer to the predictability long achieved in pre-training.

RL 레시피에 대한 대규모 Ablation. 각 선택들은 점근선 혹은 연산 효율성을 이동시킴. 최적 선택들을 결합하면 각 선택에 대한 Albation은 주로 연산 효율성과 학습 안정성을 변경함.

무엇보다 안정적인 RL 세팅을 통해 학습 초기 결과로 점근선을 외삽하는 것이 가능. RL에 대한 Scaling Law 시대의 시작?

Large scale ablations on RL recipes. Each choice shifts asymptotes or compute efficiency. When optimal choices are combined ablations on each modification mainly affect compute efficiency and training stability.

And stable RL settings allow estimation of asymptotes from early training results. The beginning of scaling laws for RL?

#rl #reasoning #scaling-law 