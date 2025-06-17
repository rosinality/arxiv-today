https://arxiv.org/abs/2402.10193

*BitDelta: Your Fine-Tune May Only Be Worth One Bit* (James Liu, Guangxuan Xiao, Kai Li, Jason D. Lee, Song Han, Tri Dao, Tianle Cai)

> Large Language Models (LLMs) are typically trained in two phases: pre-training on large internet-scale datasets, and fine-tuning for downstream tasks. Given the higher computational demand of pre-training, it's intuitive to assume that fine-tuning adds less new information to the model, and is thus more compressible. We explore this assumption by decomposing the weights of fine-tuned models into their pre-trained components and an additional delta. We introduce a simple method, BitDelta, which successfully quantizes this delta down to 1 bit without compromising performance. This interesting finding not only highlights the potential redundancy of information added during fine-tuning, but also has significant implications for the multi-tenant serving and multi-tenant storage of fine-tuned models. By enabling the use of a single high-precision base model accompanied by multiple 1-bit deltas, BitDelta dramatically reduces GPU memory requirements by more than 10x, which can also be translated to enhanced generation latency in multi-tenant settings. We validate BitDelta through experiments across Llama-2 and Mistral model families, and on models up to 70B parameters, showcasing minimal performance degradation over all tested settings.

베이스 모델과 파인튜닝한 모델의 Weight의 차이를 1 bit Quantization해서 크기를 줄이겠다는 아이디어. PEFT로 풀 파인튜닝의 효과를 도달하려고 하는 대신 풀 파인튜닝의 체크포인트 크기를 줄여보면 어떨까 하는 생각이군요.

#quantization #efficiency 