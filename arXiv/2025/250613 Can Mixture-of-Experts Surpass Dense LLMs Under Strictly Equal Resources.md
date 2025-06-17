https://arxiv.org/abs/2506.12119

*Can Mixture-of-Experts Surpass Dense LLMs Under Strictly Equal Resources?* (Houyi Li, Ka Man Lo, Ziqi Wang, Zili Wang, Wenzhen Zheng, Shuigeng Zhou, Xiangyu Zhang, Daxin Jiang)

> Mixture-of-Experts (MoE) language models dramatically expand model capacity and achieve remarkable performance without increasing per-token compute. However, can MoEs surpass dense architectures under strictly equal resource constraints - that is, when the total parameter count, training compute, and data budget are identical? This question remains under-explored despite its significant practical value and potential. In this paper, we propose a novel perspective and methodological framework to study this question thoroughly. First, we comprehensively investigate the architecture of MoEs and achieve an optimal model design that maximizes the performance. Based on this, we subsequently find that an MoE model with activation rate in an optimal region is able to outperform its dense counterpart under the same total parameter, training compute and data resource. More importantly, this optimal region remains consistent across different model sizes. Although additional amount of data turns out to be a trade-off for the enhanced performance, we show that this can be resolved via reusing data. We validate our findings through extensive experiments, training nearly 200 language models at 2B scale and over 50 at 7B scale, cumulatively processing 50 trillion tokens. All models will be released publicly.

MoE vs Dense. 총 파라미터가 동일한 경우에도 최적 아키텍처 세팅 하에서는 동일 연산량에서 MoE가 Dense보다 우수하다는 결과. 최적 아키텍처가 비전형적이긴 하네요 (K = 1). Activated Weight의 비율은 20% 정도가 최적이라는 결론.

동일 연산량이기 때문에 데이터를 더 써야 하는데 이 부분은 Multi Epoch로 극복이 가능할 것이라고 추정.

<english>
MoE vs Dense. The results insista that MoE is better than dense even with same total parameters, under optimal architectures and same computations. Optimal architecture is somewhat unconventional (K = 1). Optimal ratio of activated weight was 20%.

As it is comparison under same computation it requires more data, and they insist that it can be overcome using multi epoch.
</english>

#moe 