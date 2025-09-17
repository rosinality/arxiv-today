https://arxiv.org/abs/2508.15884

*Jet-Nemotron: Efficient Language Model with Post Neural Architecture Search* (Yuxian Gu, Qinghao Hu, Shang Yang, Haocheng Xi, Junyu Chen, Song Han, Han Cai)

> We present Jet-Nemotron, a new family of hybrid-architecture language models, which matches or exceeds the accuracy of leading full-attention models while significantly improving generation throughput. Jet-Nemotron is developed using Post Neural Architecture Search (PostNAS), a novel neural architecture exploration pipeline that enables efficient model design. Unlike prior approaches, PostNAS begins with a pre-trained full-attention model and freezes its MLP weights, allowing efficient exploration of attention block designs. The pipeline includes four key components: (1) learning optimal full-attention layer placement and elimination, (2) linear attention block selection, (3) designing new attention blocks, and (4) performing hardware-aware hyperparameter search. Our Jet-Nemotron-2B model achieves comparable or superior accuracy to Qwen3, Qwen2.5, Gemma3, and Llama3.2 across a comprehensive suite of benchmarks while delivering up to 53.6x generation throughput speedup and 6.1x prefilling speedup. It also achieves higher accuracy on MMLU and MMLU-Pro than recent advanced MoE full-attention models, such as DeepSeek-V3-Small and Moonlight, despite their larger scale with 15B total and 2.2B activated parameters.

프리트레이닝된 모델에서 FFN을 얼린 다음 Efficient Attention을 학습시키는 형태로 Efficient Attention 아키텍처와 배치를 탐색. 남겨야 하는 Attention 레이어를 찾은 다음 그 외의 레이어는 Efficient Attention으로 교체. 여기서는 Dynamic Convolution을 사용.

Search for efficient attention architectures and placement by freezing the FFN of a pretrained model and training with efficient attention. After find out crucial layers replace the remaining layers with efficient alternatives. They used dynamic convolution as the efficient alternative.

#transformer #efficient-attention #state-space-model 