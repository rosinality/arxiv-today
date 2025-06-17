https://arxiv.org/abs/2405.05254

*You Only Cache Once: Decoder-Decoder Architectures for Language Models* (Yutao Sun, Li Dong, Yi Zhu, Shaohan Huang, Wenhui Wang, Shuming Ma, Quanlu Zhang, Jianyong Wang, Furu Wei)

> We introduce a decoder-decoder architecture, YOCO, for large language models, which only caches key-value pairs once. It consists of two components, i.e., a cross-decoder stacked upon a self-decoder. The self-decoder efficiently encodes global key-value (KV) caches that are reused by the cross-decoder via cross-attention. The overall model behaves like a decoder-only Transformer, although YOCO only caches once. The design substantially reduces GPU memory demands, yet retains global attention capability. Additionally, the computation flow enables prefilling to early exit without changing the final output, thereby significantly speeding up the prefill stage. Experimental results demonstrate that YOCO achieves favorable performance compared to Transformer in various settings of scaling up model size and number of training tokens. We also extend YOCO to 1M context length with near-perfect needle retrieval accuracy. The profiling results show that YOCO improves inference memory, prefill latency, and throughput by orders of magnitude across context lengths and model sizes. Code is available at https://aka.ms/YOCO.

인코더-디코더가 이렇게 다시 등장하는군요. 인코더-디코더 구조에서 최종 레이어의 인코더 임베딩만 사용한다는 것을 일종의 Key/Value 캐시에 대한 압축처럼 사용했군요.

Causal Masking과 Efficient Attention을 사용해 디코더의 절반을 인코더처럼 임베딩을 출력하게 합니다. 이 임베딩에 대한 Cross Attention으로 나머지 디코더 절반을 구성해서 전체적으로는 하나의 디코더처럼 작동하게 만들었네요.

#efficiency