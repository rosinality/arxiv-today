https://arxiv.org/abs/2408.05636

*Speculative Diffusion Decoding: Accelerating Language Generation through Diffusion* (Jacob K Christopher, Brian R Bartoldson, Bhavya Kailkhura, Ferdinando Fioretto)

> Speculative decoding has emerged as a widely adopted method to accelerate large language model inference without sacrificing the quality of the model outputs. While this technique has facilitated notable speed improvements by enabling parallel sequence verification, its efficiency remains inherently limited by the reliance on incremental token generation in existing draft models. To overcome this limitation, this paper proposes an adaptation of speculative decoding which uses discrete diffusion models to generate draft sequences. This allows parallelization of both the drafting and verification steps, providing significant speed-ups to the inference process. Our proposed approach, \textit{Speculative Diffusion Decoding (SpecDiff)}, is validated on standard language generation benchmarks and empirically demonstrated to provide a \textbf{up to 8.7x speed-up over standard generation processes and up to 2.5x speed-up over existing speculative decoding approaches.}

Speculative Decoding에서 Drafter를 Diffusion LM으로 교체한 시도. Drafter도 병렬로 디코딩을 할 수 있으면 좋고, Verification은 Autoregressive LM으로 하면 되니 성능 문제가 없다는 아이디어군요. 신박하네요.

#efficiency 