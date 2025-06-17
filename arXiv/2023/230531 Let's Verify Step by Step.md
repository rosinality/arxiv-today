https://arxiv.org/abs/2305.20050

Let's Verify Step by Step (Hunter Lightman, Vineet Kosaraju, Yura Burda, Harri Edwards, Bowen Baker, Teddy Lee, Jan Leike, John Schulman, Ilya Sutskever, Karl Cobbe)

OpenAI의 수학 문제를 푸는 모델이군요. 중요한 포인트는 최종 결과에 대해서만 reward를 주는 것이 아니라 중간 단계들에 대해 reward를 주는 것이네요. 추가적으로 labeling 비용을 줄이기 위해 active learning을 사용했습니다. 방법은 현재 reward model이 높은 스코어를 반환하지만 최종적으로는 답이 틀린 케이스를 모아서 labeling 하는 방식이네요.

결론적으로 rlhf를 사용해 모델의 추론 능력을 향상시킬 수 있다는 증거가 되겠네요.

#alignment 