https://arxiv.org/abs/2502.08606

*Distillation Scaling Laws* (Dan Busbridge, Amitis Shidani, Floris Weers, Jason Ramapuram, Etai Littwin, Russ Webb)

> We provide a distillation scaling law that estimates distilled model performance based on a compute budget and its allocation between the student and teacher. Our findings reduce the risks associated with using distillation at scale; compute allocation for both the teacher and student models can now be done to maximize student performance. We provide compute optimal distillation recipes for when 1) a teacher exists, or 2) a teacher needs training. If many students are to be distilled, or a teacher already exists, distillation outperforms supervised pretraining until a compute level which grows predictably with student size. If one student is to be distilled and a teacher also needs training, supervised learning should be done instead. Additionally, we provide insights across our large scale study of distillation, which increase our understanding of distillation and inform experimental design.

Distillation에 대한 Scaling Law. 주요한 아이디어는 토큰 수가 충분하다면 Distillation이 아니라 일반적인 프리트레이닝이 더 낫다, 따라서 Distillation이 나은 조건과 (예를 들어 Teacher 모델이 이미 있는 경우) 데이터의 양을 결정해야 한다는 것이라고 할 수 있겠네요.

<english>
Scaling law for distillation. The main idea is plain pretraining is better than distillation when number of training token is enough. Therefore we should decide in what situations (for example, when we already have teacher model) and amount of data distillation would worker bettern thain plain training.
</english>

#distillation #scaling-law 