https://arxiv.org/abs/2501.02423

*Scaling Laws for Floating Point Quantization Training* (Xingwu Sun, Shuaipeng Li, Ruobing Xie, Weidong Han, Kan Wu, Zhen Yang, Yixing Li, An Wang, Shuai Li, Jinbao Xue, Yu Cheng, Yangyu Tao, Zhanhui Kang, Chengzhong Xu, Di Wang, Jie Jiang)

> Low-precision training is considered an effective strategy for reducing both training and downstream inference costs. Previous scaling laws for precision mainly focus on integer quantization, which pay less attention to the constituents in floating-point quantization and thus cannot well fit the LLM losses in this scenario. In contrast, while floating-point quantization training is more commonly implemented in production, the research on it has been relatively superficial. In this paper, we thoroughly explore the effects of floating-point quantization targets, exponent bits, mantissa bits, and the calculation granularity of the scaling factor in floating-point quantization training performance of LLM models. While presenting an accurate floating-point quantization unified scaling law, we also provide valuable suggestions for the community: (1) Exponent bits contribute slightly more to the model performance than mantissa bits. We provide the optimal exponent-mantissa bit ratio for different bit numbers, which is available for future reference by hardware manufacturers; (2) We discover the formation of the critical data size in low-precision LLM training. Too much training data exceeding the critical data size will inversely bring in degradation of LLM performance; (3) The optimal floating-point quantization precision is directly proportional to the computational power, but within a wide computational power range, we estimate that the best cost-performance precision lies between 4-8 bits.

Quantized Training에 대한 Scaling Law. Bit width에 따른 최적 Exponent/Mantissa 등 재미있는 부분이 많네요. 그런데 여기서 사용한 Scaling Law의 함수형에 따르면 특정 Precision에서 추가로 학습하면 오히려 Validation Loss가 상승하는 변곡점이 발생합니다. 좀 낯선 아이디어군요.

<english>
Scaling law for quantized training. There are many interesting points like optiomal exponent/mantissa assignment for specific bit widths. But if we follow functional form of scaling law used in here, it suggest that there exists inflection point that further training increase validation loss for specific precision. I think it is somewhat odd idea.
</english>

#quantization #scaling-law 