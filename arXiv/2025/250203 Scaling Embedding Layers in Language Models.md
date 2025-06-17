https://arxiv.org/abs/2502.01637

*Scaling Embedding Layers in Language Models* (Da Yu, Edith Cohen, Badih Ghazi, Yangsibo Huang, Pritish Kamath, Ravi Kumar, Daogao Liu, Chiyuan Zhang)

> We propose SCONE ($\textbf{S}$calable, $\textbf{C}$ontextualized, $\textbf{O}$ffloaded, $\textbf{N}$-gram $\textbf{E}$mbedding), a method for extending input embedding layers to enhance language model performance as layer size scales. To avoid increased decoding costs, SCONE retains the original vocabulary while introducing embeddings for a set of frequent $n$-grams. These embeddings provide contextualized representation for each input token and are learned with a separate model during training. During inference, they are precomputed and stored in off-accelerator memory with minimal impact on inference speed. SCONE enables two new scaling strategies: increasing the number of cached $n$-gram embeddings and scaling the model used to learn them, all while maintaining fixed inference-time FLOPS. We show that scaling both aspects allows SCONE to outperform a 1.9B parameter baseline across diverse corpora, while using only half the inference-time FLOPS.

n-gram 임베딩을 사용한 모델. 얼마 전 비슷한 아이디어가 나왔었죠. (https://arxiv.org/abs/2501.16975) 이쪽은 n-gram 임베딩을 트랜스포머로 출력하게 했네요. 추론 시에는 n-gram 임베딩을 캐시에 저장해놓을 수 있으니 괜찮다는 발상입니다.

<english>
A model with n-gram embeddings. Recently similar idea was presented (https://arxiv.org/abs/2501.16975). This work let transformer to output n-gram embeddings. The idea is it could be efficient as we can save n-gram embedding in cache for inference.
</english>

#embedding #lm

# Links

[[250128 Over-Tokenized Transformer.md]]