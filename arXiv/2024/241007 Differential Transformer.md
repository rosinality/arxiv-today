https://arxiv.org/abs/2410.05258

*Differential Transformer* (Tianzhu Ye, Li Dong, Yuqing Xia, Yutao Sun, Yi Zhu, Gao Huang, Furu Wei)

> Transformer tends to overallocate attention to irrelevant context. In this work, we introduce Diff Transformer, which amplifies attention to the relevant context while canceling noise. Specifically, the differential attention mechanism calculates attention scores as the difference between two separate softmax attention maps. The subtraction cancels noise, promoting the emergence of sparse attention patterns. Experimental results on language modeling show that Diff Transformer outperforms Transformer in various settings of scaling up model size and training tokens. More intriguingly, it offers notable advantages in practical applications, such as long-context modeling, key information retrieval, hallucination mitigation, in-context learning, and reduction of activation outliers. By being less distracted by irrelevant context, Diff Transformer can mitigate hallucination in question answering and text summarization. For in-context learning, Diff Transformer not only enhances accuracy but is also more robust to order permutation, which was considered as a chronic robustness issue. The results position Diff Transformer as a highly effective and promising architecture to advance large language models.

불필요한 토큰에 Attention Weight가 주어지는 현상이 문제라는 아이디어. 이에 대해 Attention Score의 차이를 사용하는 방법을 생각했군요. Attention의 엔트로피가 문제라는 것은 이전에도 제기된 문제였고 (https://arxiv.org/abs/2308.16137) 최근에도 이야기가 나오고 있죠. (https://arxiv.org/abs/2410.01104) 이에 대한 해결책은 뚜렷하지 않았는데 한 가지 방법이 등장했군요.

<english>
The idea that attention weight is assigned to the unnecessary tokens. The paper devised the method that using the difference between attention scores. There was previous results that says entropy of attention is problematic (https://arxiv.org/abs/2308.16137), it is also recently discussed (https://arxiv.org/abs/2410.01104). There was no straightforward solution for this, but one is appeared with this paper.
</english>

#transformer #long-context #attention

# Links

[[230830 LM-Infinite.md]]