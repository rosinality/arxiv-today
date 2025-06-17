https://arxiv.org/abs/2405.01535

*Prometheus 2: An Open Source Language Model Specialized in Evaluating Other Language Models* (Seungone Kim, Juyoung Suk, Shayne Longpre, Bill Yuchen Lin, Jamin Shin, Sean Welleck, Graham Neubig, Moontae Lee, Kyungjae Lee, Minjoon Seo)

> Proprietary LMs such as GPT-4 are often employed to assess the quality of responses from various LMs. However, concerns including transparency, controllability, and affordability strongly motivate the development of open-source LMs specialized in evaluations. On the other hand, existing open evaluator LMs exhibit critical shortcomings: 1) they issue scores that significantly diverge from those assigned by humans, and 2) they lack the flexibility to perform both direct assessment and pairwise ranking, the two most prevalent forms of assessment. Additionally, they do not possess the ability to evaluate based on custom evaluation criteria, focusing instead on general attributes like helpfulness and harmlessness. To address these issues, we introduce Prometheus 2, a more powerful evaluator LM than its predecessor that closely mirrors human and GPT-4 judgements. Moreover, it is capable of processing both direct assessment and pair-wise ranking formats grouped with a user-defined evaluation criteria. On four direct assessment benchmarks and four pairwise ranking benchmarks, Prometheus 2 scores the highest correlation and agreement with humans and proprietary LM judges among all tested open evaluator LMs. Our models, code, and data are all publicly available at https://github.com/prometheus-eval/prometheus-eval.

Prometheus 2가 나왔군요. 여기서 메인은 Pairwise Ranking에 대한 지원인 듯 한데 Direct Assessment와 Pairwise Ranking을 동시에 지원하기 위해 Joint Training을 넘어 Weight Merging을 시도했다는 게 재미있네요.

Llama 2 Chat, Mistral 7B Instruct, Mixtral 8x7B Instruct를 사용했는데 Llama 3 70B 수준으로 넘어간다면 굉장히 강력한 평가 모델이 나올지도 모르겠다 싶네요.

#evaluation 