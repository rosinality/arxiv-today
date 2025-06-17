https://arxiv.org/abs/2504.16980

*Safety Pretraining: Toward the Next Generation of Safe AI* (Pratyush Maini, Sachin Goyal, Dylan Sam, Alex Robey, Yash Savani, Yiding Jiang, Andy Zou, Zacharcy C. Lipton, J. Zico Kolter)

> As large language models (LLMs) are increasingly deployed in high-stakes settings, the risk of generating harmful or toxic content remains a central challenge. Post-hoc alignment methods are brittle: once unsafe patterns are learned during pretraining, they are hard to remove. We present a data-centric pretraining framework that builds safety into the model from the start. Our contributions include: (i) a safety classifier trained on 10,000 GPT-4 labeled examples, used to filter 600B tokens; (ii) the largest synthetic safety dataset to date (100B tokens) generated via recontextualization of harmful web data; (iii) RefuseWeb and Moral Education datasets that convert harmful prompts into refusal dialogues and web-style educational material; (iv) Harmfulness-Tag annotations injected during pretraining to flag unsafe content and steer away inference from harmful generations; and (v) safety evaluations measuring base model behavior before instruction tuning. Our safety-pretrained models reduce attack success rates from 38.8% to 8.4% with no performance degradation on standard LLM safety benchmarks.

프리트레이닝 데이터에서 안전 문제가 있는 텍스트를 재작성해 오히려 윤리를 가르치는 텍스트로 바꿔 학습시킨 시도. 텍스트를 버리는 것보다는 이쪽이 낫지 않을까 싶습니다. 물론 저는 나쁜 것도 아는 것이 모르는 것보다는 낫지 않나 하는 생각을 합니다만.

<english>
Attempt to training LLM using rewriting unsafe data into moral education data, instead of filter out it. I think it is better than just remove the texts. Actually, I think it is better to know about bad things, instead of does not aware of it at all.
</english>

#safety #pretraining 