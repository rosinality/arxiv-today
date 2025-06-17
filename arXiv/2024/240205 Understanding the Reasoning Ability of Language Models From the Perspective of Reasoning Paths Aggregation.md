https://arxiv.org/abs/2402.03268

*Understanding the Reasoning Ability of Language Models From the Perspective of Reasoning Paths Aggregation* (Xinyi Wang, Alfonso Amayuelas, Kexun Zhang, Liangming Pan, Wenhu Chen, William Yang Wang)

> Pre-trained language models (LMs) are able to perform complex reasoning without explicit fine-tuning. To understand how pre-training with a next-token prediction objective contributes to the emergence of such reasoning capability, we propose that we can view an LM as deriving new conclusions by aggregating indirect reasoning paths seen at pre-training time. We found this perspective effective in two important cases of reasoning: logic reasoning with knowledge graphs (KGs) and math reasoning with math word problems (MWPs). More specifically, we formalize the reasoning paths as random walk paths on the knowledge/reasoning graphs. Analyses of learned LM distributions suggest that a weighted sum of relevant random walk path probabilities is a reasonable way to explain how LMs reason. Experiments and analysis on multiple KG and MWP datasets reveal the effect of training on random walk paths and suggest that augmenting unlabeled random walk reasoning paths can improve real-world multi-step reasoning performance.

LLM에서 추론 능력이 어떻게 발생하는가? 이 논문에서는 엔티티 노드들이 관계로 연결된 그래프를 생각합니다. 그리고 이 그래프 위에서 랜덤 워크를 통해 경유한 노드와 관계로 시퀀스를 만들어 학습 데이터를 만들죠.

그리고 이에 대해 LM 학습을 했을 때 엔티티들의 연결 경로들을 합쳐서 추론하는 알고리즘과 비슷하게 작동할 수 있다는 아이디어입니다.

#reasoning #lm 