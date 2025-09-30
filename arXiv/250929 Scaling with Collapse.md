https://arxiv.org/abs/2509.25087

*Scaling with Collapse: Efficient and Predictable Training of LLM Families* (Shane Bergsma, Bin Claire Zhang, Nolan Dey, Shaheer Muhammad, Gurpreet Gosal, Joel Hestness)

> Effective LLM training relies on *consistency*, meaning that key quantities -- such as final losses and optimal hyperparameters -- scale predictably across model sizes. Qiu et al. (2025) recently showed that this consistency extends beyond scalars: whole training loss curves can *collapse* onto a universal trajectory after a simple normalization. What remains unclear is whether this phenomenon holds for LLM families trained under *practical scaling recipes*, where width, depth, learning rate, batch size, and weight decay are scaled jointly. We show that it does: loss curves collapse across scales precisely when optimization hyperparameters are set optimally for the given data budget, in accordance with recent empirical scaling laws. Collapse thus emerges as a signature of compute-efficient training. We demonstrate two applications at scale: (1) deviation-from-collapse provides a sensitive, early diagnostic of training pathologies, and (2) the predictability of collapsed curves enables early stopping in large-scale hyperparameter tuning. Finally, we train a competitive LLM family, *Celerity*, using these insights, highlighting collapse as an effective tool for developing efficient LLMs.

최종 Loss로 나눠주면 Loss 커브의 개형이 일치한다는 결과에 대한 확장 (https://arxiv.org/abs/2507.02119). 토큰 대 파라미터 비율과 최적화의 타임스케일, LR 스케줄이 일치하면 Loss 커브의 일치가 일어난다는 것을 발견. 따라서 전체 학습 커브가 작은 규모의 학습을 통해 예측 가능함. 

<english>
Expansion of the result of collapse of loss curves into same form if it is divided by the final loss (https://arxiv.org/abs/2507.02119). They found that if token-per-parameter ratio and timescale of optimization, LR schedule is same then collapse occurs. Thus entire training trajectory is predictable from the smaller training runs.
</english>

#scaling-law #optimization 