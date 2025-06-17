https://arxiv.org/abs/2309.10202

Stabilizing RLHF through Advantage Model and Selective Rehearsal (Baolin Peng, Linfeng Song, Ye Tian, Lifeng Jin, Haitao Mi, Dong Yu)

reward score의 분포가 데이터의 특정 카테고리마다 제각각일 수 있기 때문에 높은 스코어 분포를 보이는 카테고리의 특성이 낮은 스코어 분포의 카테고리에게로 전이되어서 reward hacking이 일어난다는 문제, 그리고 ppo 과정에서 획득했던 스킬들이 소실된다는 문제에 대한 대응이군요.

reward score 분포 문제는 reward score에 advantage model을 적용하는 것으로 대응했습니다. 스킬들이 소실되는 문제는 ppo training dataset의 prompt-response 페어들을 클러스터링하고 거기에서 대표 샘플을 뽑은 다음, ppo 과정 중에 이 샘플들로 autoregressive loss를 첨가하는 식으로 대응했습니다. InstructGPT에서 ppo에 추가로 pretraining loss를 붙였던 것을 연상시키네요.

#rl #alignment #instruction-tuning 