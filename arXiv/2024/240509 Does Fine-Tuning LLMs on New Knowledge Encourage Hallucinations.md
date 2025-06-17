https://arxiv.org/abs/2405.05904

*Does Fine-Tuning LLMs on New Knowledge Encourage Hallucinations?* (Zorik Gekhman, Gal Yona, Roee Aharoni, Matan Eyal, Amir Feder, Roi Reichart, Jonathan Herzig)

> When large language models are aligned via supervised fine-tuning, they may encounter new factual information that was not acquired through pre-training. It is often conjectured that this can teach the model the behavior of hallucinating factually incorrect responses, as the model is trained to generate facts that are not grounded in its pre-existing knowledge. In this work, we study the impact of such exposure to new knowledge on the capability of the fine-tuned model to utilize its pre-existing knowledge. To this end, we design a controlled setup, focused on closed-book QA, where we vary the proportion of the fine-tuning examples that introduce new knowledge. We demonstrate that large language models struggle to acquire new factual knowledge through fine-tuning, as fine-tuning examples that introduce new knowledge are learned significantly slower than those consistent with the model's knowledge. However, we also find that as the examples with new knowledge are eventually learned, they linearly increase the model's tendency to hallucinate. Taken together, our results highlight the risk in introducing new factual knowledge through fine-tuning, and support the view that large language models mostly acquire factual knowledge through pre-training, whereas fine-tuning teaches them to use it more efficiently.

LLM이 모르는 지식으로 파인튜닝을 하는 것이 할루시네이션을 유발하는가라는 문제에 대한 연구. 통제된 세팅에서 LLM이 아는 지식과 모르는 지식의 비율과 학습량을 바꿔가면서 테스트해봤네요.

요약하자면 모르는 지식에 대해서는 학습 속도가 느리고 학습을 하는 시점에서는 오버핏을 유발한다고 말하고 있습니다. 아는 지식에 대해서 학습이 빠르고 성능이 더 나은 특성을 보이네요.

새삼 Schulman이 SFT vs RLHF를 논하면서 굉장히 이른 시점에 중요한 문제에 대한 통찰을 제공한 것 같다 싶습니다. (https://www.youtube.com/watch?v=hhiLw5Q_UFg)

#alignment #hallucination 