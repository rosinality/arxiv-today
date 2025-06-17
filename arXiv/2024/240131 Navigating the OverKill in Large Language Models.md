https://arxiv.org/abs/2401.17633

*Navigating the OverKill in Large Language Models* (Chenyu Shi, Xiao Wang, Qiming Ge, Songyang Gao, Xianjun Yang, Tao Gui, Qi Zhang, Xuanjing Huang, Xun Zhao, Dahua Lin)

> Large language models are meticulously aligned to be both helpful and harmless. However, recent research points to a potential overkill which means models may refuse to answer benign queries. In this paper, we investigate the factors for overkill by exploring how models handle and determine the safety of queries. Our findings reveal the presence of shortcuts within models, leading to an over-attention of harmful words like 'kill' and prompts emphasizing safety will exacerbate overkill. Based on these insights, we introduce Self-Contrastive Decoding (Self-CD), a training-free and model-agnostic strategy, to alleviate this phenomenon. We first extract such over-attention by amplifying the difference in the model's output distributions when responding to system prompts that either include or omit an emphasis on safety. Then we determine the final next-token predictions by downplaying the over-attention from the model via contrastive decoding. Empirical results indicate that our method has achieved an average reduction of the refusal rate by 20\% while having almost no impact on safety.

프로세스를 kill 하라고 했을 때 응답을 거부하지 않는가는 요즘 LLM들의 통과 의례죠. 여기서는 맥락과는 별개로 개별 단어에 LLM이 너무 꽂히는 것이 문제인 것 같다고 보고, 그래서 Safety 프롬프트를 추가한 경우의 응답과의 Contrast를 통해서 이런 경향을 억제하는 방법을 테스트해봤습니다.

맥락이 아니라 개별 단어라는 것이 시사하듯 모델의 Capacity와 관련된 문제라는 생각이 많이 들긴 하네요. 물론 다양한 맥락 Instruction을 쓰는 것도 도움이 되겠지만요.

#safety 

It is a gateway question for LLMs now a days that asking kill a process. In this study LLMs overly concentrate on specific words instead of semantic contexts. Therefore this study proposes method that applying contrastive decoding between plain LLM decodings respect to decodings that safety prompt appended.

The notion that word instead of contexts imply that this problem is related to capacity of LLMs. Anyway using instructions with various contextual cases will be helpful.