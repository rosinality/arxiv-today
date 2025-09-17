https://arxiv.org/abs/2507.18578

*Wide-In, Narrow-Out: Revokable Decoding for Efficient and Effective DLLMs* (Feng Hong, Geng Yu, Yushi Ye, Haicheng Huang, Huangjie Zheng, Ya Zhang, Yanfeng Wang, Jiangchao Yao)

> Diffusion Large Language Models (DLLMs) have emerged as a compelling alternative to Autoregressive models, designed for fast parallel generation. However, existing DLLMs are plagued by a severe quality-speed trade-off, where faster parallel decoding leads to significant performance degradation. We attribute this to the irreversibility of standard decoding in DLLMs, which is easily polarized into the wrong decoding direction along with early error context accumulation. To resolve this, we introduce Wide-In, Narrow-Out (WINO), a training-free decoding algorithm that enables revokable decoding in DLLMs. WINO employs a parallel draft-and-verify mechanism, aggressively drafting multiple tokens while simultaneously using the model's bidirectional context to verify and re-mask suspicious ones for refinement. Verified in open-source DLLMs like LLaDA and MMaDA, WINO is shown to decisively improve the quality-speed trade-off. For instance, on the GSM8K math benchmark, it accelerates inference by 6$\times$ while improving accuracy by 2.58%; on Flickr30K captioning, it achieves a 10$\times$ speedup with higher performance. More comprehensive experiments are conducted to demonstrate the superiority and provide an in-depth understanding of WINO.

Diffusion LM에서 생성한 토큰을 수정할 수 있도록 하는 디코딩 방법. 검증 방법이 재미있음. 마스크 토큰 시퀀스를 시퀀스 끝에 붙여서 디코딩했을 때 기존 토큰과 같은 토큰이 나오는지 확인.

A decoding method that allows diffusion LMs to revoke tokens. The verification method is interesting. It appends a masked token sequence to the end and checks whether the same tokens as the existing ones are generated.

#diffusion #decoding 