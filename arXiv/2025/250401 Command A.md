https://arxiv.org/abs/2504.00698

*Command A: An Enterprise-Ready Large Language Model* (Cohere)

> In this report we describe the development of Command A, a powerful large language model purpose-built to excel at real-world enterprise use cases. Command A is an agent-optimised and multilingual-capable model, with support for 23 languages of global business, and a novel hybrid architecture balancing efficiency with top of the range performance. It offers best-in-class Retrieval Augmented Generation (RAG) capabilities with grounding and tool use to automate sophisticated business processes. These abilities are achieved through a decentralised training approach, including self-refinement algorithms and model merging techniques. We also include results for Command R7B which shares capability and architectural similarities to Command A. Weights for both models have been released for research purposes. This technical report details our original training pipeline and presents an extensive evaluation of our models across a suite of enterprise-relevant tasks and public benchmarks, demonstrating excellent performance and efficiency.

Cohere에서 얼마 전 공개했던 Command A에 대해 리포트를 냈네요. 흥미롭게도 H100 클러스터에서 JAX로 학습을 했군요.

포스트트레이닝에 대해서 비교적 자세한데 한 가지, 코드 실행 결과를 프리트레이닝 데이터로 사용했다는 언급이 있네요.

<english>
Cohere published report for Command A they released recently. Interestingly, they did training using JAX on H100 clusters.

It is rather detailed on post-training, but one point, they mentions that they used code execution results as a pretraining data.
</english>

#llm #pretraining #post-training 