https://arxiv.org/abs/2410.07167

*Deciphering Cross-Modal Alignment in Large Vision-Language Models with Modality Integration Rate* (Qidong Huang, Xiaoyi Dong, Pan Zhang, Yuhang Zang, Yuhang Cao, Jiaqi Wang, Dahua Lin, Weiming Zhang, Nenghai Yu)

> We present the Modality Integration Rate (MIR), an effective, robust, and generalized metric to indicate the multi-modal pre-training quality of Large Vision Language Models (LVLMs). Large-scale pre-training plays a critical role in building capable LVLMs, while evaluating its training quality without the costly supervised fine-tuning stage is under-explored. Loss, perplexity, and in-context evaluation results are commonly used pre-training metrics for Large Language Models (LLMs), while we observed that these metrics are less indicative when aligning a well-trained LLM with a new modality. Due to the lack of proper metrics, the research of LVLMs in the critical pre-training stage is hindered greatly, including the training data choice, efficient module design, etc. In this paper, we propose evaluating the pre-training quality from the inter-modal distribution distance perspective and present MIR, the Modality Integration Rate, which is 1) \textbf{Effective} to represent the pre-training quality and show a positive relation with the benchmark performance after supervised fine-tuning. 2) \textbf{Robust} toward different training/evaluation data. 3) \textbf{Generalize} across training configurations and architecture choices. We conduct a series of pre-training experiments to explore the effectiveness of MIR and observe satisfactory results that MIR is indicative about training data selection, training strategy schedule, and model architecture design to get better pre-training results. We hope MIR could be a helpful metric for building capable LVLMs and inspire the following research about modality alignment in different areas. Our code is at: https://github.com/shikiw/Modality-Integration-Rate.

이미지 토큰과 텍스트 토큰의 분포의 유사도가 (FID) 모델의 성능과 연관성이 높다는 아이디어. 재미있네요. Loss와 비슷한 느낌이지만 Loss보다 좀 더 강인한 지표일 수 있다는 이야기를 합니다.

<english>
The idea that similarity of distribution (FID) between image and text tokens is highly correlated with model performances. it feels similar to the loss, but they say that it is more robust metric compared to the loss.
</english>

#multimodal #metric 