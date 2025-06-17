https://arxiv.org/abs/2308.13137

OmniQuant: Omnidirectionally Calibrated Quantization for Large Language Models (Wenqi Shao, Mengzhao Chen, Zhaoyang Zhang, Peng Xu, Lirui Zhao, Zhiqian Li, Kaipeng Zhang, Peng Gao, Yu Qiao, Ping Luo)

weight quantization 방법. quantization에서 발생하는 error를 보정하기 위한 튜닝, dynamic range 학습, smoothquant처럼 activation에서 발생하는 outlier 문제를 weight로 이전하는 트릭을 결합했군요.

llama 시리즈에 대해 결과는 흥미롭네요. 다만 quantization을 적용하기 전에 우리가 perplexity 0.1의 의미가 무엇인지 충분히 이해하고 있는 것인지 의문스럽다는 생각이 요즘 드네요.

#quantization 