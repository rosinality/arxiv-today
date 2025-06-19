https://arxiv.org/abs/2506.15211

*ProtoReasoning: Prototypes as the Foundation for Generalizable Reasoning in LLMs* (Feng He, Zijun Chen, Xinnian Liang, Tingting Ma, Yunqi Qiu, Shuangzhi Wu, Junchi Yan)

> Recent advances in Large Reasoning Models (LRMs) trained with Long Chain-of-Thought (Long CoT) reasoning have demonstrated remarkable cross-domain generalization capabilities. However, the underlying mechanisms supporting such transfer remain poorly understood. We hypothesize that cross-domain generalization arises from shared abstract reasoning prototypes -- fundamental reasoning patterns that capture the essence of problems across domains. These prototypes minimize the nuances of the representation, revealing that seemingly diverse tasks are grounded in shared reasoning structures.Based on this hypothesis, we propose ProtoReasoning, a framework that enhances the reasoning ability of LLMs by leveraging scalable and verifiable prototypical representations (Prolog for logical reasoning, PDDL for planning).ProtoReasoning features: (1) an automated prototype construction pipeline that transforms problems into corresponding prototype representations; (2) a comprehensive verification system providing reliable feedback through Prolog/PDDL interpreters; (3) the scalability to synthesize problems arbitrarily within prototype space while ensuring correctness. Extensive experiments show that ProtoReasoning achieves 4.7% improvement over baseline models on logical reasoning (Enigmata-Eval), 6.3% improvement on planning tasks, 4.0% improvement on general reasoning (MMLU) and 1.0% on mathematics (AIME24). Significantly, our ablation studies confirm that learning in prototype space also demonstrates enhanced generalization to structurally similar problems compared to training solely on natural language representations, validating our hypothesis that reasoning prototypes serve as the foundation for generalizable reasoning in large language models.

프롤로그 같은 언어로 논리 추론을 학습시키면 이 추론 능력이 다른 도메인에서도 작동하지 않겠는가 하는 아이디어. 다양한 도메인과 Verifier를 사용하는 것은 좋은 일이겠죠. 물론 그 모든 것을 통합하는 Objective가 있을지도 모르겠습니다만.

하루키, 토우마, 세츠나가 대체 누구인가 했는데 꽤 고전적인 게임의 캐릭터들인 것 같군요.

<english>
The idea of training logical reasoning using languages like Prolog may develop transferable reasoning capabilities that could work on the other domains. It is nice thing to use diverse domains and verifiers. Of course, there could be an objective that unifies all of them.

I wondered who is Haruki, Touma, Setsuna, and found ther

#reasoning #rl 