https://arxiv.org/abs/2408.11796

*LLM Pruning and Distillation in Practice: The Minitron Approach* (Sharath Turuvekere Sreenivas, Saurav Muralidharan, Raviraj Joshi, Marcin Chochowski, Mostofa Patwary, Mohammad Shoeybi, Bryan Catanzaro, Jan Kautz, Pavlo Molchanov)

> We present a comprehensive report on compressing the Llama 3.1 8B and Mistral NeMo 12B models to 4B and 8B parameters, respectively, using pruning and distillation. We explore two distinct pruning strategies: (1) depth pruning and (2) joint hidden/attention/MLP (width) pruning, and evaluate the results on common benchmarks from the LM Evaluation Harness. The models are then aligned with NeMo Aligner and tested in instruct-tuned versions. This approach produces a compelling 4B model from Llama 3.1 8B and a state-of-the-art Mistral-NeMo-Minitron-8B (MN-Minitron-8B for brevity) model from Mistral NeMo 12B. We found that with no access to the original data, it is beneficial to slightly fine-tune teacher models on the distillation dataset. We open-source our base model weights on Hugging Face with a permissive license.

NVIDIA가 Distillation을 사용한 모델 압축을 요즘 열심히 하는군요. 이전에도 논문을 하나 냈었는데 (https://arxiv.org/abs/2407.14679) 이쪽의 중요한 차이는 학습 데이터를 모르는 외부 모델을 사용해 Distill을 하기 위해 Teacher 모델을 가지고 있는 데이터에 튜닝하는 단계를 거친다는 것이네요.

#distillation #pruning

# Links

[[240719 Compact Language Models via Pruning and Knowledge Distillation.md]]