https://arxiv.org/abs/2503.10061

*Compute Optimal Scaling of Skills: Knowledge vs Reasoning* (Nicholas Roberts, Niladri Chatterji, Sharan Narang, Mike Lewis, Dieuwke Hupkes)

> Scaling laws are a critical component of the LLM development pipeline, most famously as a way to forecast training decisions such as 'compute-optimally' trading-off parameter count and dataset size, alongside a more recent growing list of other crucial decisions. In this work, we ask whether compute-optimal scaling behaviour can be skill-dependent. In particular, we examine knowledge and reasoning-based skills such as knowledge-based QA and code generation, and we answer this question in the affirmative: scaling laws are skill-dependent. Next, to understand whether skill-dependent scaling is an artefact of the pretraining datamix, we conduct an extensive ablation of different datamixes and find that, also when correcting for datamix differences, knowledge and code exhibit fundamental differences in scaling behaviour. We conclude with an analysis of how our findings relate to standard compute-optimal scaling using a validation set, and find that a misspecified validation set can impact compute-optimal parameter count by nearly 50%, depending on its skill composition.

Scaling Law를 추정할 때 Validation으로 지식 관련 데이터를 사용하는가, 코딩 관련 데이터를 사용하는가에 따라서 Compute Optimal 지점의 파라미터와 데이터 할당 비율이 달라진다는 연구. 지식 관련에서는 파라미터에, 코딩 관련에서는 데이터에 더 할당하게 되는군요. 흥미로운 결과네요.

This study shows that the compute optimal allocation of parameter and data varies depending on whether knowledge-related or code-related data is used for validation when estimating scaling law. When using knowledge-related validation data more compute is allocated to parameters, while with code-related validation data, more is allocated to data size. Intriguing results.

#scaling-law 