https://arxiv.org/abs/2505.07796

*Learning Dynamics in Continual Pre-Training for Large Language Models* (Xingjin Wang, Howe Tissue, Lu Wang, Linjing Li, Daniel Dajun Zeng)

> Continual Pre-Training (CPT) has become a popular and effective method to apply strong foundation models to specific downstream tasks. In this work, we explore the learning dynamics throughout the CPT process for large language models. We specifically focus on how general and downstream domain performance evolves at each training step, with domain performance measured via validation losses. We have observed that the CPT loss curve fundamentally characterizes the transition from one curve to another hidden curve, and could be described by decoupling the effects of distribution shift and learning rate annealing. We derive a CPT scaling law that combines the two factors, enabling the prediction of loss at any (continual) training steps and across learning rate schedules (LRS) in CPT. Our formulation presents a comprehensive understanding of several critical factors in CPT, including loss potential, peak learning rate, training steps, replay ratio, etc. Moreover, our approach can be adapted to customize training hyper-parameters to different CPT goals such as balancing general and domain-specific performance. Extensive experiments demonstrate that our scaling law holds across various CPT datasets and training hyper-parameters.

Continual Pretraining에 대한 Scaling Law. LR Annealing에 의한 항과 Distribution Shift에 의한 항으로 구성되는군요.

<english>
A scaling law for continual pretraining. It is consists of term on LR annealing and distribution shift.
</english>

#continual-learning #scaling-law 