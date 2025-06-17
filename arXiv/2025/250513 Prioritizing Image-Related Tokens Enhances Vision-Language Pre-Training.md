https://arxiv.org/abs/2505.08971

*Prioritizing Image-Related Tokens Enhances Vision-Language Pre-Training* (Yangyi Chen, Hao Peng, Tong Zhang, Heng Ji)

> In standard large vision-language models (LVLMs) pre-training, the model typically maximizes the joint probability of the caption conditioned on the image via next-token prediction (NTP); however, since only a small subset of caption tokens directly relates to the visual content, this naive NTP unintentionally fits the model to noise and increases the risk of hallucination. We present PRIOR, a simple vision-language pre-training approach that addresses this issue by prioritizing image-related tokens through differential weighting in the NTP loss, drawing from the importance sampling framework. PRIOR introduces a reference model-a text-only large language model (LLM) trained on the captions without image inputs, to weight each token based on its probability for LVLMs training. Intuitively, tokens that are directly related to the visual inputs are harder to predict without the image and thus receive lower probabilities from the text-only reference LLM. During training, we implement a token-specific re-weighting term based on the importance scores to adjust each token's loss. We implement PRIOR in two distinct settings: LVLMs with visual encoders and LVLMs without visual encoders. We observe 19% and 8% average relative improvement, respectively, on several vision-language benchmarks compared to NTP. In addition, PRIOR exhibits superior scaling properties, as demonstrated by significantly higher scaling coefficients, indicating greater potential for performance gains compared to NTP given increasing compute and data.

텍스트만으로는 예측하기 어려운 토큰들이 이미지 관련 토큰이라고 생각하고 가중치를 준다는 아이디어. Rho Loss가 생각나네요.

<english>
The idea of up-weights tokens hard to predict only with texts by considering it as an image-related tokens. It reminds me Rho loss.
</english>

#multimodal 