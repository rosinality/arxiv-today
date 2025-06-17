https://arxiv.org/abs/2411.16035

*Predicting Emergent Capabilities by Finetuning* (Charlie Snell, Eric Wallace, Dan Klein, Sergey Levine)

> A fundamental open challenge in modern LLM scaling is the lack of understanding around emergent capabilities. In particular, language model pretraining loss is known to be highly predictable as a function of compute. However, downstream capabilities are far less predictable -- sometimes even exhibiting emergent jumps -- which makes it challenging to anticipate the capabilities of future models. In this work, we first pose the task of emergence prediction: given access to current LLMs that have random few-shot accuracy on a task, can we predict whether future models (GPT-N+1) will have non-trivial accuracy on that task? We then discover a simple insight for this problem: finetuning LLMs on a given task can shift the point in scaling at which emergence occurs towards less capable models. To operationalize this insight, we can finetune LLMs with varying amounts of data and fit a parametric function that predicts when emergence will occur (i.e., "emergence laws"). We validate this approach using four standard NLP benchmarks where large-scale open-source LLMs already demonstrate emergence (MMLU, GSM8K, CommonsenseQA, and CoLA). Using only small-scale LLMs, we find that, in some cases, we can accurately predict whether models trained with up to 4x more compute have emerged. Finally, we present a case study of two realistic uses for emergence prediction.

현재 랜덤 성능이 나오는 모델만이 있을 때 어느 시점에서 Emergence가 발생하는지를 예측할 수 있는지에 대한 문제. 파인튜닝을 했을 때 Emergence가 발생하는 지점이 이동하고, 또 파인튜닝 데이터의 규모 증가에 따라 이 이동이 비례한다는 것을 기반으로 모델링을 했습니다. 파인튜닝 데이터의 양에 따른 Emergence 지점에 대한 공식이 있다면 파인튜닝 데이터의 양을 0으로 지정했을 때 나오는 지점이 Few-shot에서 Emergence가 발생하는 지점이라는 것이죠.

<english>
The problem of predicting point of emergence when we can only access to the model which has random accuracy. Modeled this based on the fact that point of emergence is left shifts when finetuned, and the degree of the shift is determined by the size of the finetuning data. If we have formula for the point of emergence that depends on the size of the finetuning data, then we can get the point of emergence of few-shot cases by letting the size of finetuing to 0.
</english>

#scaling-law 