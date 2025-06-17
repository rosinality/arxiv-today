https://arxiv.org/abs/2410.14268

*MoDification: Mixture of Depths Made Easy* (Chen Zhang, Meizhi Zhong, Qimeng Wang, Xuantao Lu, Zheyu Ye, Chengqiang Lu, Yan Gao, Yao Hu, Kehai Chen, Min Zhang, Dawei Song)

> Long-context efficiency has recently become a trending topic in serving large language models (LLMs). And mixture of depths (MoD) is proposed as a perfect fit to bring down both latency and memory. In this paper, however, we discover that MoD can barely transform existing LLMs without costly training over an extensive number of tokens. To enable the transformations from any LLMs to MoD ones, we showcase top-k operator in MoD should be promoted to threshold-p operator, and refinement to architecture and data should also be crafted along. All these designs form our method termed MoDification. Through a comprehensive set of experiments covering model scales from 3B to 70B, we exhibit MoDification strikes an excellent balance between efficiency and effectiveness. MoDification can achieve up to ~1.2x speedup in latency and ~1.8x reduction in memory compared to original LLMs especially in long-context applications.

Mixture of Depths에서 Top-K 대신 확률에 대한 Threshold를 사용하자는 아이디어. Mixture of Depths 원 논문에서 Autoregressive 세팅을 위해 Predictor를 사용한 것과 비슷할 것 같네요.

<english>
The idea that use probability threshold for mixture of depths instead of top-K. It is similar to using predictor in original mixture of depths paper for autoregressive models
</english>

#moe 