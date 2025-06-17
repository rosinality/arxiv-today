https://arxiv.org/abs/2409.13198

*Exploring Scaling Laws for Local SGD in Large Language Model Training* (Qiaozhi He, Xiaomin Zhuang, Zhihua Wu)

> This paper investigates scaling laws for local SGD in LLM training, a distributed optimization algorithm that facilitates training on loosely connected devices. Through extensive experiments, we show that local SGD achieves competitive results compared to conventional methods, given equivalent model parameters, datasets, and computational resources. Furthermore, we explore the application of local SGD in various practical scenarios, including multi-cluster setups and edge computing environments. Our findings elucidate the necessary conditions for effective multi-cluster LLM training and examine the potential and limitations of leveraging edge computing resources in the LLM training process. This demonstrates its viability as an alternative to single large-cluster training.

Local SGD에 대한 Scaling Law. Local SGD로 인해 발생하는 수렴에서의 페널티를 고려하는 Scaling Law입니다. 그리고 이 페널티를 효율성에 대한 함수로 정의했네요.

Async Training을 Scaling에서 발생하는 문제에 대한 대안으로 연구하고 있다는 이야기들이 있긴 하더군요. 지금까지 그렇게 좋은 결과가 있었던 문제는 아니지만...붙잡고 계속 파다보면 뭔가 성과가 나올지도 모르겠네요. (성과가 나오는 즉시 영업 기밀 취급이 될 것 같긴 합니다만.)

#scaling-law #efficient-training 