https://arxiv.org/abs/2404.10830

*Fewer Truncations Improve Language Modeling* (Hantian Ding, Zijian Wang, Giovanni Paolini, Varun Kumar, Anoop Deoras, Dan Roth, Stefano Soatto)

> In large language model training, input documents are typically concatenated together and then split into sequences of equal length to avoid padding tokens. Despite its efficiency, the concatenation approach compromises data integrity -- it inevitably breaks many documents into incomplete pieces, leading to excessive truncations that hinder the model from learning to compose logically coherent and factually consistent content that is grounded on the complete context. To address the issue, we propose Best-fit Packing, a scalable and efficient method that packs documents into training sequences through length-aware combinatorial optimization. Our method completely eliminates unnecessary truncations while retaining the same training efficiency as concatenation. Empirical results from both text and code pre-training show that our method achieves superior performance (e.g., relatively +4.7% on reading comprehension; +16.8% in context following; and +9.2% on program synthesis), and reduces closed-domain hallucination effectively by up to 58.3%.

LLM 프리트레이닝 시점에서 문서를 이어붙인 다음 시퀀스 길이 제한에 맞게 자르다보니 문서가 잘려나가는 경우가 많으니 문서가 절단되는 경우를 줄이도록 패킹한다는 아이디어. 재미있네요.

#llm #pretraining 