https://arxiv.org/abs/2404.03862

*Verifiable by Design: Aligning Language Models to Quote from Pre-Training Data* (Jingyu Zhang, Marc Marone, Tianjian Li, Benjamin Van Durme, Daniel Khashabi)

> For humans to trust the fluent generations of large language models (LLMs), they must be able to verify their correctness against trusted, external sources. Recent efforts aim to increase verifiability through citations of retrieved documents or post-hoc provenance. However, such citations are prone to mistakes that further complicate their verifiability. To address these limitations, we tackle the verifiability goal with a different philosophy: we trivialize the verification process by developing models that quote verbatim statements from trusted sources in pre-training data. We propose Quote-Tuning, which demonstrates the feasibility of aligning LLMs to leverage memorized information and quote from pre-training data. Quote-Tuning quantifies quoting against large corpora with efficient membership inference tools, and uses the amount of quotes as an implicit reward signal to construct a synthetic preference dataset for quoting, without any human annotation. Next, the target model is aligned to quote using preference optimization algorithms. Experimental results show that Quote-Tuning significantly increases the percentage of LLM generation quoted verbatim from high-quality pre-training documents by 55% to 130% relative to untuned models while maintaining response quality. Further experiments demonstrate that Quote-Tuning generalizes quoting to out-of-domain data, is applicable in different tasks, and provides additional benefits to truthfulness. Quote-Tuning not only serves as a hassle-free method to increase quoting but also opens up avenues for improving LLM trustworthiness through better verifiability.

답변 생성 시 최대한 코퍼스에서 텍스트를 그대로 사용한 텍스트를 작성하도록 유도하는 방법. n-gram에 대해서 n-gram이 코퍼스에 등장하는가를 Reward로 사용해서 학습시키는 방법입니다. 문서 ID를 응답에 포함시키도록 하는 방법도 최근 나왔는데 (https://arxiv.org/abs/2404.01019) 재미있네요.

#instruction-tuning

# Links

[[240401 Source-Aware Training Enables Knowledge Attribution in Language Models.md]]