https://arxiv.org/abs/2405.14591

*Base of RoPE Bounds Context Length* (Xin Men, Mingyu Xu, Bingning Wang, Qingyu Zhang, Hongyu Lin, Xianpei Han, Weipeng Chen)

> Position embedding is a core component of current Large Language Models (LLMs). Rotary position embedding (RoPE), a technique that encodes the position information with a rotation matrix, has been the de facto choice for position embedding in many LLMs, such as the Llama series. RoPE has been further utilized to extend long context capability, which is roughly based on adjusting the \textit{base} parameter of RoPE to mitigate out-of-distribution (OOD) problems in position embedding. However, in this paper, we find that LLMs may obtain a superficial long-context ability based on the OOD theory. We revisit the role of RoPE in LLMs and propose a novel property of long-term decay, we derive that the \textit{base of RoPE bounds context length}: there is an absolute lower bound for the base value to obtain certain context length capability. Our work reveals the relationship between context length and RoPE base both theoretically and empirically, which may shed light on future long context training.

RoPE의 base 파라미터를 Context Length에 따라 어떻게 설정해야 하는가에 대한 체계적인 연구가 나왔네요. Long Context를 제대로 활용해야 한다, 더 구체적으로는 가까운 토큰에 집중하고 쿼리와 유사한 토큰을 잘 구분할 수 있어야 한다는 조건 하에서 Context Length를 실제로 잘 활용하기 위한 base의 최저선을 설정하는 형태입니다. 경험적으로 세팅해왔던 부분인데 흥미로운 진전인 것 같습니다.

#positional-encoding #long-context 