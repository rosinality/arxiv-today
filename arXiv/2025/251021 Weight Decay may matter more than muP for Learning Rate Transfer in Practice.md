https://arxiv.org/abs/2510.19093

*Weight Decay may matter more than muP for Learning Rate Transfer in Practice* (Atli Kosson, Jeremy Welborn, Yang Liu, Martin Jaggi, Xi Chen)

> Transferring the optimal learning rate from small to large neural networks can enable efficient training at scales where hyperparameter tuning is otherwise prohibitively expensive. To this end, the Maximal Update Parameterization (muP) proposes a learning rate scaling designed to keep the update dynamics of internal representations stable across different model widths. However, the scaling rules of muP rely on strong assumptions, particularly about the geometric alignment of a layer's inputs with both its weights and gradient updates. In this large-scale empirical investigation, we show that these assumptions hold only briefly at the start of training in the practical setups where learning rate transfer is most valuable, such as LLM training. For the remainder of training it is weight decay rather than muP that correctly stabilizes the update dynamics of internal representations across widths, facilitating learning rate transfer. This suggests muP's scaling primarily acts as a form of implicit learning rate warmup, allowing us to largely replace it with modified warmup schedules. Together these findings fundamentally challenge prevailing beliefs about learning rate transfer and can explain empirical practice such as why muP requires the independent weight decay variant for successful transfer.

μP와 Weight Decay 문제. LR Transfer를 위해서 μP에 추가적으로 Independent Weight Decay가 필요한 이유는 무엇인가? μP의 정렬 가정은 학습의 초반에만 성립. 학습의 나머지 기간 동안 Relative Weight 변화를 유지하기 위해선 Weight Decay가 그 역할을 해야함.

μP and weight decay problem, again. Why μP requires independent weight decay for LR transfer? μP's alignment assumption is only satisfied at the early period of the training. To keep relative weight changes for the rest of the training weight decay should play the role.

#optimization 