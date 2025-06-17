https://arxiv.org/abs/2404.05892

*Eagle and Finch: RWKV with Matrix-Valued States and Dynamic Recurrence* (Bo Peng, Daniel Goldstein, Quentin Anthony, Alon Albalak, Eric Alcaide, Stella Biderman, Eugene Cheah, Teddy Ferdinan, Haowen Hou, Przemysław Kazienko, Kranthi Kiran GV, Jan Kocoń, Bartłomiej Koptyra, Satyapriya Krishna, Ronald McClelland Jr., Niklas Muennighoff, Fares Obeid, Atsushi Saito, Guangyu Song, Haoqin Tu, Stanisław Woźniak, Ruichong Zhang, Bingchen Zhao, Qihang Zhao, Peng Zhou, Jian Zhu, Rui-Jie Zhu)

> We present Eagle (RWKV-5) and Finch (RWKV-6), sequence models improving upon the RWKV (RWKV-4) architecture. Our architectural design advancements include multi-headed matrix-valued states and a dynamic recurrence mechanism that improve expressivity while maintaining the inference efficiency characteristics of RNNs. We introduce a new multilingual corpus with 1.12 trillion tokens and a fast tokenizer based on greedy matching for enhanced multilinguality. We trained four Eagle models, ranging from 0.46 to 7.5 billion parameters, and two Finch models with 1.6 and 3.1 billion parameters and find that they achieve competitive performance across a wide variety of benchmarks. We release all our models on HuggingFace under the Apache 2.0 license. Models at: https://huggingface.co/RWKV Training code at: https://github.com/RWKV/RWKV-LM Inference code at: https://github.com/RWKV/ChatRWKV Time-parallel training code at: https://github.com/RWKV/RWKV-infctx-trainer

RWKV-5와 6에 대한 리포트도 나왔군요. SSM의 추세처럼 행렬 형태의 상태를 채택한 것이 가장 큰 변화인 것 같습니다. 그런데 6 같은 경우엔 여러 모듈이 붙어 꽤 복잡하네요. 과거 스타일의 모델 아키텍처의 향수가 느껴지기도 하고 그렇습니다.

Associative Recall에서는 꽤 괜찮은 결과를 보여주고 있습니다. 다만 Based 같은 경우를 보면 Information Extraction 과제로 테스트하면 차이가 드러나더군요. (https://arxiv.org/abs/2402.18668) 이 부분이 흥미로운 과제가 될 것 같네요.

#state-space-model

# Links

