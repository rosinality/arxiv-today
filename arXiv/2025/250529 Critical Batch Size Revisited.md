https://arxiv.org/abs/2505.23971

*Critical Batch Size Revisited: A Simple Empirical Approach to Large-Batch Language Model Training* (William Merrill, Shane Arora, Dirk Groeneveld, Hannaneh Hajishirzi)

> The right batch size is important when training language models at scale: a large batch size is necessary for fast training, but a batch size that is too large will harm token efficiency. To navigate this tradeoff, McCandlish et al. (2018) suggest that a critical batch size (CBS), below which training will not substantially degrade loss, can be estimated based on the gradient noise scale during training. While their method has been adopted in practice, e.g., when training GPT-3, strong assumptions are required to justify gradient noise as a proxy for the CBS, which makes it unclear whether their approach should be trusted in practice, limiting its applicability. In this paper, we introduce a simple, empirical approach to directly measure the CBS and show how the CBS evolves over training. Applying our approach to the OLMo models, we find that CBS is near 0 at initialization, increases rapidly at first, and then plateaus as training progresses. Furthermore, we find that this trend holds across different model sizes (1B and 7B), suggesting CBS from small training runs can inform larger-scale training runs. Our findings about how the CBS changes over training motivate batch size warmup as a natural way to reliably train language models at large batch size: start the batch size small and increase it as the CBS grows. To validate this claim, we use batch size warmup to train OLMo 1B to slightly better loss than the original training run with 43% fewer gradient steps. This shows how our framework can be applied to reliably train language models at larger batch sizes, increasing data parallelism without compromising performance.

Critical Batch Size를 모델 학습 과정에서 추정할 수 있는 방법을 만들었네요.

<english>
A method of estimating critical batch sizes for each training steps.
</english>

#optimization 