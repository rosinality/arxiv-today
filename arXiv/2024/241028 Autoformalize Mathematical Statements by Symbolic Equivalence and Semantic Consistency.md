https://arxiv.org/abs/2410.20936

*Autoformalize Mathematical Statements by Symbolic Equivalence and Semantic Consistency* (Zenan Li, Yifan Wu, Zhaoyu Li, Xinming Wei, Xian Zhang, Fan Yang, Xiaoxing Ma)

> Autoformalization, the task of automatically translating natural language descriptions into a formal language, poses a significant challenge across various domains, especially in mathematics. Recent advancements in large language models (LLMs) have unveiled their promising capabilities to formalize even competition-level math problems. However, we observe a considerable discrepancy between pass@1 and pass@k accuracies in LLM-generated formalizations. To address this gap, we introduce a novel framework that scores and selects the best result from k autoformalization candidates based on two complementary self-consistency methods: symbolic equivalence and semantic consistency. Elaborately, symbolic equivalence identifies the logical homogeneity among autoformalization candidates using automated theorem provers, and semantic consistency evaluates the preservation of the original meaning by informalizing the candidates and computing the similarity between the embeddings of the original and informalized texts. Our extensive experiments on the MATH and miniF2F datasets demonstrate that our approach significantly enhances autoformalization accuracy, achieving up to 0.22-1.35x relative improvements across various LLMs and baseline methods.

Autoformalization을 위한 Self Consistency 방법 연구. 논리적으로 같은가를 Proof Assistant로 체크, Informal하게 다시 변환했을 때 의미적으로 원문과 같은가를 체크.

Proof Assistant를 Reward로 활용하려는 시도에서 Autoformalization은 같이 등장하는 주제이지만 이 방법이 정말로 나아갈 방향인가에 대한 고민은 필요할 것 같네요.

<english>
Self consistency methods for autoformalization. Checking logical equivalence using proof assistant, and it is semantically similar to original texts if it is transformed into informal statements.

Autoformalization is theme occurs with approaches that tries to use proof assistant as a reward function. But whether this approach is viable for teaching reasoning to model needs consideration.
</english>

#reasoning #math 