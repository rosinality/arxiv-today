https://arxiv.org/abs/2405.21060

*Transformers are SSMs: Generalized Models and Efficient Algorithms Through Structured State Space Duality* (Tri Dao, Albert Gu)

> While Transformers have been the main architecture behind deep learning's success in language modeling, state-space models (SSMs) such as Mamba have recently been shown to match or outperform Transformers at small to medium scale. We show that these families of models are actually quite closely related, and develop a rich framework of theoretical connections between SSMs and variants of attention, connected through various decompositions of a well-studied class of structured semiseparable matrices. Our state space duality (SSD) framework allows us to design a new architecture (Mamba-2) whose core layer is an a refinement of Mamba's selective SSM that is 2-8X faster, while continuing to be competitive with Transformers on language modeling.

State Space Model들을 (L◦QK^T)V 형태로 생각했을 때 L 행렬에 부여하는 구조에 따라 Linear Attention, Retentive Network 등등 다양한 모델들이 유도된다는 아이디어. 여기서는 1-Semiseparable이라는 구조를 고려합니다.

이를 통해 얻을 수 있는 것은 State Space Model과 Attention을 하나로 연결해 계산 과정에서 일부는 Attention 형태로 계산하고 부분적으로 Recurrent하게 계산하는 방식으로 연산 효율성을 높일 수 있다는 것이네요. 기존의 Mamba와 비슷하거나 더 나은 성능을 확보하면서 Long Context에 대해 더 빠른 연산이 가능합니다.

#state-space-model 