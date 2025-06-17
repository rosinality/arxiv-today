https://arxiv.org/abs/2409.04410

*Open-MAGVIT2: An Open-Source Project Toward Democratizing Auto-regressive Visual Generation* (Zhuoyan Luo, Fengyuan Shi, Yixiao Ge, Yujiu Yang, Limin Wang, Ying Shan)

> We present Open-MAGVIT2, a family of auto-regressive image generation models ranging from 300M to 1.5B. The Open-MAGVIT2 project produces an open-source replication of Google's MAGVIT-v2 tokenizer, a tokenizer with a super-large codebook (i.e., $2^{18}$ codes), and achieves the state-of-the-art reconstruction performance (1.17 rFID) on ImageNet $256 \times 256$. Furthermore, we explore its application in plain auto-regressive models and validate scalability properties. To assist auto-regressive models in predicting with a super-large vocabulary, we factorize it into two sub-vocabulary of different sizes by asymmetric token factorization, and further introduce "next sub-token prediction" to enhance sub-token interaction for better generation quality. We release all models and codes to foster innovation and creativity in the field of auto-regressive visual generation.

Large Vocabulary Vector Quantization을 적용한 Autoregressive Image Generation 모델들이 드디어 등장했군요. Look-up Free Quantization을 사용해 Vocabulary를 2^18 = 262K로 증가시켰습니다.

다만 262K Vocabulary를 직접 모델링한 것은 아니고 Vocabulary를 Factorize해서 쪼갠 다음 입력으로는 이 Factorize된 Vocabulary의 합을 사용하고 출력 시에 Factorize된 Vocabulary들을 순차적으로 생성하는 방식을 사용했네요.

#vq #autoregressive-model #image-generation 