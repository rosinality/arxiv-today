https://arxiv.org/abs/2403.08730

*Strengthening Multimodal Large Language Model with Bootstrapped Preference Optimization* (Renjie Pi, Tianyang Han, Wei Xiong, Jipeng Zhang, Runtao Liu, Rui Pan, Tong Zhang)

> Multimodal Large Language Models (MLLMs) excel in generating responses based on visual inputs. However, they often suffer from a bias towards generating responses similar to their pretraining corpus, overshadowing the importance of visual information. We treat this bias as a "preference" for pretraining statistics, which hinders the model's grounding in visual input. To mitigate this issue, we propose Bootstrapped Preference Optimization (BPO), which conducts preference learning with datasets containing negative responses bootstrapped from the model itself. Specifically, we propose the following two strategies: 1) using distorted image inputs to the MLLM for eliciting responses that contain signified pretraining bias; 2) leveraging text-based LLM to explicitly inject erroneous but common elements into the original response. Those undesirable responses are paired with original annotated responses from the datasets to construct the preference dataset, which is subsequently utilized to perform preference learning. Our approach effectively suppresses pretrained LLM bias, enabling enhanced grounding in visual inputs. Extensive experimentation demonstrates significant performance improvements across multiple benchmarks, advancing the state-of-the-art in multimodal conversational systems.

이미지-텍스트 Alignment는 텍스트 프리트레이닝에 비해 규모가 작기에 Vision-Language 모델은 여전히 텍스트 프리트레이닝의 영향을 크게 받고 있고 따라서 이미지에 제대로 Grounding 되어 있지 않고 대신 텍스트적인 특성에 따라 생성하는 경향이 많다는 아이디어.

대응 방안은 Golden Label을 Positive로 하고 이미지에 노이즈를 넣어 할루시네이션을 유도한 샘플들, LLM으로 텍스트를 변조한 샘플들을 Negative로 설정해서 DPO를 했습니다.

결국 RL을 하자는 결론이 다시 나왔군요.

#hallucination #rlaif