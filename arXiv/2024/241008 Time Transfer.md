https://arxiv.org/abs/2410.05838

*Time Transfer: On Optimal Learning Rate and Batch Size In The Infinite Data Limit* (Oleg Filatov, Jan Ebert, Jiangtao Wang, Stefan Kesselheim)

> One of the main challenges in optimal scaling of large language models (LLMs) is the prohibitive cost of hyperparameter tuning, particularly learning rate $\eta$ and batch size $B$. While techniques like $\mu$P (Yang et al., 2022) provide scaling rules for optimal $\eta$ transfer in the infinite model size limit, the optimal scaling behavior in the infinite data size limit ($T \to \infty$) remains unknown. We fill in this gap by observing for the first time an interplay of three optimal $\eta$ scaling regimes: $\eta \propto \sqrt{T}$, $\eta \propto 1$, and $\eta \propto 1/\sqrt{T}$ with transitions controlled by $B$ and its relation to the time-evolving critical batch size $B_\mathrm{crit} \propto T$. Furthermore, we show that the optimal batch size is positively correlated with $B_\mathrm{crit}$: keeping it fixed becomes suboptimal over time even if learning rate is scaled optimally. Surprisingly, our results demonstrate that the observed optimal $\eta$ and $B$ dynamics are preserved with $\mu$P model scaling, challenging the conventional view of $B_\mathrm{crit}$ dependence solely on loss value. Complementing optimality, we examine the sensitivity of loss to changes in learning rate, where we find the sensitivity to decrease with $T \to \infty$ and to remain constant with $\mu$P model scaling. We hope our results make the first step towards a unified picture of the joint optimal data and model scaling.

요즘 자주 이야기가 나오는 학습량 증가에 따른 최적 LR과 배치 크기의 변화. LR과 배치 크기의 상호작용이 있어서 해석이 복잡하긴 한데 일단 최적 Loss 타겟에서는 학습량에 따라 LR과 배치 크기가 단조 증가하는 것 같네요.

문제가 복잡해지긴 하지만 그래도 다행스러운 것은 학습량 증가에 따라 LR에 대한 민감도가 감소하는 것 같다는 것이네요. μP도 모델 크기 증가에 따른 영향을 제거하는데 성공했습니다.

<english>
The changes in optimal LR and batch sizes according to increase of training time, which is discussed recently. It is hard to analyze because of the interaction between LR and batch sizes, but it seems like that LR and batch size is monotonically increasing with longer trainings for optimal loss targets.

It makes the problem complex, but relievely, sensitivity of LR is decreasing along with training durations, and μP was successful to remove the effect of model size increment.
</english>

#hyperparameter #scaling-law 