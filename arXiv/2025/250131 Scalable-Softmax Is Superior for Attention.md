https://arxiv.org/abs/2501.19399

*Scalable-Softmax Is Superior for Attention* (Ken M. Nakanishi)

> The maximum element of the vector output by the Softmax function approaches zero as the input vector size increases. Transformer-based language models rely on Softmax to compute attention scores, causing the attention distribution to flatten as the context size grows. This reduces the model's ability to prioritize key information effectively and potentially limits its length generalization. To address this problem, we propose Scalable-Softmax (SSMax), which replaces Softmax in scenarios where the input vector size varies. SSMax can be seamlessly integrated into existing Transformer-based architectures. Experimental results in language modeling show that models using SSMax not only achieve faster loss reduction during pretraining but also significantly improve performance in long contexts and key information retrieval. Furthermore, an analysis of attention scores reveals that SSMax enables the model to focus attention on key information even in long contexts. Additionally, although models that use SSMax from the beginning of pretraining achieve better length generalization, those that have already started pretraining can still gain some of this ability by replacing Softmax in the attention layers with SSMax, either during or after pretraining.

Softmax의 Logit에 길이에 따라 증가하는 계수 log n을 붙여 엔트로피 증가를 억제하는 방식으로 Long Context Extrapolation을 시도.

<english>
A method for long context extrapolation by suppressing increase of entropy by add scalar that increase with sequence length (log n) to logit in softmax.
</english>

#long-context 