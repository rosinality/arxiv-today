https://arxiv.org/abs/2405.01481

*NeMo-Aligner: Scalable Toolkit for Efficient Model Alignment* (Gerald Shen, Zhilin Wang, Olivier Delalleau, Jiaqi Zeng, Yi Dong, Daniel Egert, Shengyang Sun, Jimmy Zhang, Sahil Jain, Ali Taghibakhshi, Markel Sanz Ausin, Ashwath Aithal, Oleksii Kuchaiev)

> Aligning Large Language Models (LLMs) with human values and preferences is essential for making them helpful and safe. However, building efficient tools to perform alignment can be challenging, especially for the largest and most competent LLMs which often contain tens or hundreds of billions of parameters. We create NeMo-Aligner, a toolkit for model alignment that can efficiently scale to using hundreds of GPUs for training. NeMo-Aligner comes with highly optimized and scalable implementations for major paradigms of model alignment such as: Reinforcement Learning from Human Feedback (RLHF), Direct Preference Optimization (DPO), SteerLM, and Self-Play Fine-Tuning (SPIN). Additionally, our toolkit supports running most of the alignment techniques in a Parameter Efficient Fine-Tuning (PEFT) setting. NeMo-Aligner is designed for extensibility, allowing support for other alignment techniques with minimal effort. It is open-sourced with Apache 2.0 License and we invite community contributions at https://github.com/NVIDIA/NeMo-Aligner

NVIDIA의 정렬 프레임워크. 가장 중요한 부분은 샘플링을 어떻게 처리했는가일 텐데 TensorRT를 썼다고 하네요.

Llama 3 400B가 나오면 정렬 측면에서도 좀 더 까다로운 부분들이 생길테니 미리 준비하는 것도 좋을 듯 합니다.

#alignment 