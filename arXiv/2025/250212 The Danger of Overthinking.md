https://arxiv.org/abs/2502.08235

*The Danger of Overthinking: Examining the Reasoning-Action Dilemma in Agentic Tasks* (Alejandro Cuadron, Dacheng Li, Wenjie Ma, Xingyao Wang, Yichuan Wang, Siyuan Zhuang, Shu Liu, Luis Gaspar Schroeder, Tian Xia, Huanzhi Mao, Nicholas Thumiger, Aditya Desai, Ion Stoica, Ana Klimovic, Graham Neubig, Joseph E. Gonzalez)

> Large Reasoning Models (LRMs) represent a breakthrough in AI problem-solving capabilities, but their effectiveness in interactive environments can be limited. This paper introduces and analyzes overthinking in LRMs. A phenomenon where models favor extended internal reasoning chains over environmental interaction. Through experiments on software engineering tasks using SWE Bench Verified, we observe three recurring patterns: Analysis Paralysis, Rogue Actions, and Premature Disengagement. We propose a framework to study these behaviors, which correlates with human expert assessments, and analyze 4018 trajectories. We observe that higher overthinking scores correlate with decreased performance, with reasoning models exhibiting stronger tendencies toward overthinking compared to non-reasoning models. Our analysis reveals that simple efforts to mitigate overthinking in agentic environments, such as selecting the solution with the lower overthinking score, can improve model performance by almost 30% while reducing computational costs by 43%. These results suggest that mitigating overthinking has strong practical implications. We suggest that by leveraging native function-calling capabilities and selective reinforcement learning overthinking tendencies could be mitigated. We also open-source our evaluation framework and dataset to facilitate research in this direction at https://github.com/AlexCuadron/Overthinking.

모델에 추론 능력이 생기면서 에이전트가 행동하는 대신 생각하는 시간만 지나치게 길어질 수 있다는 아이디어. 재미있는 문제의식이네요. 물론 사고의 길이와 오류율을 단순하게 연결시킬 수는 없겠죠.

이에 대한 대응으로 가장 쉽게 생각할 수 있는 것은 RL 과정에서 중간에 모델이 행동을 할 수 있게 허용하는 것이겠네요.

<english>
As model now have reasoning ability, the idea of agent might just think long instead of actually doing an action. It is interesting concept of problem. Of course it is not straightforward to connect length of thoughts and error rates.

Naturally solution for this problem to allow model to do an action in intermediate steps while doing RL.
</english>

#reasoning #agent 