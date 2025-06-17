https://arxiv.org/abs/2412.18860

*Bootstrap Your Own Context Length* (Liang Wang, Nan Yang, Xingxing Zhang, Xiaolong Huang, Furu Wei)

> We introduce a bootstrapping approach to train long-context language models by exploiting their short-context capabilities only. Our method utilizes a simple agent workflow to synthesize diverse long-context instruction tuning data, thereby eliminating the necessity for manual data collection and annotation. The proposed data synthesis workflow requires only a short-context language model, a text retriever, and a document collection, all of which are readily accessible within the open-source ecosystem. Subsequently, language models are fine-tuned using the synthesized data to extend their context lengths. In this manner, we effectively transfer the short-context capabilities of language models to long-context scenarios through a bootstrapping process. We conduct experiments with the open-source Llama-3 family of models and demonstrate that our method can successfully extend the context length to up to 1M tokens, achieving superior performance across various benchmarks.

Long Context Instruction Tuning. 프롬프트 증폭, 관련 문서 검색, 프롬프트와 관련된 내용 요약, 프롬프트와 요약을 기반으로 최종 응답 생성의 순서로 데이터를 구축하는군요.

<english>
Long-context instruction tuning. It synthesizes data in the step of prompt expansion, retrieving relevant documents, summarizing the information relevant to the prompt, generating final response based on prompt and summarization.
</english>

#long-context #instruction-tuning 