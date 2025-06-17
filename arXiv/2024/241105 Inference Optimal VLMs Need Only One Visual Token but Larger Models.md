https://arxiv.org/abs/2411.03312

*Inference Optimal VLMs Need Only One Visual Token but Larger Models* (Kevin Y. Li, Sachin Goyal, Joao D. Semedo, J. Zico Kolter)

> Vision Language Models (VLMs) have demonstrated strong capabilities across various visual understanding and reasoning tasks. However, their real-world deployment is often constrained by high latency during inference due to substantial compute required to process the large number of input tokens (predominantly from the image) by the LLM. To reduce inference costs, one can either downsize the LLM or reduce the number of input image-tokens, the latter of which has been the focus of many recent works around token compression. However, it is unclear what the optimal trade-off is, as both the factors directly affect the VLM performance. We first characterize this optimal trade-off between the number of visual tokens and LLM parameters by establishing scaling laws that capture variations in performance with these two factors. Our results reveal a surprising trend: for visual reasoning tasks, the inference-optimal behavior in VLMs, i.e., minimum downstream error at any given fixed inference compute, is achieved when using the largest LLM that fits within the inference budget while minimizing visual token count - often to a single token. While the token reduction literature has mainly focused on maintaining base model performance by modestly reducing the token count (e.g., $5-10\times$), our results indicate that the compute-optimal inference regime requires operating under even higher token compression ratios. Based on these insights, we take some initial steps towards building approaches tailored for high token compression settings. Code is available at https://github.com/locuslab/llava-token-compression.

이미지 토큰 수와 모델 크기의 트레이드오프 사이에서의 최적점을 Scaling Law로 탐색. 놀랍게도 토큰 수는 크게 줄이고 (1!) 모델을 키우는 것이 최적이었다고 하네요. 그렇지만 OCR에서는 모델 크기보다는 토큰 수가 성능을 결정했다고 합니다. 이미지 문제에서 언제나 엣지 케이스를 담당하고 있는 것이 OCR이죠.

<english>
Exploring optimal point on the trade-off between number of image tokens and model sizes using scaling law. Surprisingly, it is optimal to reduce number of tokens to the extreme (1!) and increasing the model sizes. But in OCR number of tokens tend to determine the performances rather than model sizes. OCR is always an edge case of image related tasks.
</english>

#vision-language #ocr #scaling-law 