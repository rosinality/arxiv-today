https://arxiv.org/abs/2507.09404

*Scaling Laws for Optimal Data Mixtures* (Mustafa Shukor, Louis Bethune, Dan Busbridge, David Grangier, Enrico Fini, Alaaeldin El-Nouby, Pierre Ablin)

> Large foundation models are typically trained on data from multiple domains, with the data mixture--the proportion of each domain used--playing a critical role in model performance. The standard approach to selecting this mixture relies on trial and error, which becomes impractical for large-scale pretraining. We propose a systematic method to determine the optimal data mixture for any target domain using scaling laws. Our approach accurately predicts the loss of a model of size $N$ trained with $D$ tokens and a specific domain weight vector $h$. We validate the universality of these scaling laws by demonstrating their predictive power in three distinct and large-scale settings: large language model (LLM), native multimodal model (NMM), and large vision models (LVM) pretraining. We further show that these scaling laws can extrapolate to new data mixtures and across scales: their parameters can be accurately estimated using a few small-scale training runs, and used to estimate the performance at larger scales and unseen domain weights. The scaling laws allow to derive the optimal domain weights for any target domain under a given training budget ($N$,$D$), providing a principled alternative to costly trial-and-error methods.

Scaling Law를 사용한 프리트레이닝 데이터 비율 결정.

<english>
Determining ratio of pretraining data mixtures using scaling law.
</english>

#pretraining #multimodal #scaling-law #dataset 