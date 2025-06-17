https://arxiv.org/abs/2501.18965

*The Surprising Agreement Between Convex Optimization Theory and Learning-Rate Scheduling for Large Model Training* (Fabian Schaipp, Alexander Hägele, Adrien Taylor, Umut Simsekli, Francis Bach)

> We show that learning-rate schedules for large model training behave surprisingly similar to a performance bound from non-smooth convex optimization theory. We provide a bound for the constant schedule with linear cooldown; in particular, the practical benefit of cooldown is reflected in the bound due to the absence of logarithmic terms. Further, we show that this surprisingly close match between optimization theory and practice can be exploited for learning-rate tuning: we achieve noticeable improvements for training 124M and 210M Llama-type models by (i) extending the schedule for continued training with optimal learning-rate, and (ii) transferring the optimal learning-rate across schedules.

Last iterate bound가 (https://arxiv.org/abs/2310.07831) 모델 학습 과정의 Loss 커브와 개형이 유사하다는 분석. 이를 기반으로 Cooldown의 비율이 어떠해야 하는지 등을 분석했군요.

LR Annealing에 대한 Scaling Law가 (https://arxiv.org/abs/2408.11029) 생각나는군요.

<english>
The analysis suggest last iterate bound (https://arxiv.org/abs/2310.07831) is similar to loss curve during model training in shape. They analzed the problems like how we should set proportion of cooldown based on this.

It reminds me scaling law for LR annealing (https://arxiv.org/abs/2408.11029).
</english>

#optimizer

# Links

[[240820 Scaling Law with Learning Rate Annealing.md]]