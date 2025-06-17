https://arxiv.org/abs/2505.04741

*When Bad Data Leads to Good Models* (Kenneth Li, Yida Chen, Fernanda Viégas, Martin Wattenberg)

> In large language model (LLM) pretraining, data quality is believed to determine model quality. In this paper, we re-examine the notion of "quality" from the perspective of pre- and post-training co-design. Specifically, we explore the possibility that pre-training on more toxic data can lead to better control in post-training, ultimately decreasing a model's output toxicity. First, we use a toy experiment to study how data composition affects the geometry of features in the representation space. Next, through controlled experiments with Olmo-1B models trained on varying ratios of clean and toxic data, we find that the concept of toxicity enjoys a less entangled linear representation as the proportion of toxic data increases. Furthermore, we show that although toxic data increases the generational toxicity of the base model, it also makes the toxicity easier to remove. Evaluations on Toxigen and Real Toxicity Prompts demonstrate that models trained on toxic data achieve a better trade-off between reducing generational toxicity and preserving general capabilities when detoxifying techniques such as inference-time intervention (ITI) are applied. Our findings suggest that, with post-training taken into account, bad data may lead to good models.

유해한 데이터를 학습하는 것이 유해성을 더 잘 구분하고 정렬하는데 도움이 될 수 있다는 연구. 유해한 것을 모르는 것보다는 아는 것이 낫고 유해하게 행동하지 않게 하는 것에 집중하는 것이 나을 것 같다는 생각을 합니다.

<english>
The research suggest that training on toxic data can be beneficial to separate toxicity and aligning the model. I think it is better to know about toxic things compared to ignorant against it, and it would be better focus on behavioral aspect of model.
</english>

#pretraining #corpus #safety 