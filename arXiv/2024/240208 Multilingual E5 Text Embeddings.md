https://arxiv.org/abs/2402.05672

*Multilingual E5 Text Embeddings: A Technical Report* (Liang Wang, Nan Yang, Xiaolong Huang, Linjun Yang, Rangan Majumder, Furu Wei)

> This technical report presents the training methodology and evaluation results of the open-source multilingual E5 text embedding models, released in mid-2023. Three embedding models of different sizes (small / base / large) are provided, offering a balance between the inference efficiency and embedding quality. The training procedure adheres to the English E5 model recipe, involving contrastive pre-training on 1 billion multilingual text pairs, followed by fine-tuning on a combination of labeled datasets. Additionally, we introduce a new instruction-tuned embedding model, whose performance is on par with state-of-the-art, English-only models of similar sizes. Information regarding the model release can be found at https://github.com/microsoft/unilm/tree/master/e5 .

E5 + 생성 데이터 (https://arxiv.org/abs/2401.00368) 추가로 구축한 다국어 E5. LLM과 함께 좋은 Retriever도 중요한 시점이죠.

#retrieval 

Multilingual built with E5 and synthetic generated data. Retriever is importatnt as well as LLMs in these days.

# Links

[[231231 Improving Text Embeddings with Large Language Models.md]]