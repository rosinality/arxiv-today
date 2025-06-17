https://arxiv.org/abs/2412.04703

*Transformers Struggle to Learn to Search* (Abulhair Saparov, Srushti Pawar, Shreyas Pimpalgaonkar, Nitish Joshi, Richard Yuanzhe Pang, Vishakh Padmakumar, Seyed Mehran Kazemi, Najoung Kim, He He)

> Search is an ability foundational in many important tasks, and recent studies have shown that large language models (LLMs) struggle to perform search robustly. It is unknown whether this inability is due to a lack of data, insufficient model parameters, or fundamental limitations of the transformer architecture. In this work, we use the foundational graph connectivity problem as a testbed to generate effectively limitless high-coverage data to train small transformers and test whether they can learn to perform search. We find that, when given the right training distribution, the transformer is able to learn to search. We analyze the algorithm that the transformer has learned through a novel mechanistic interpretability technique that enables us to extract the computation graph from the trained model. We find that for each vertex in the input graph, transformers compute the set of vertices reachable from that vertex. Each layer then progressively expands these sets, allowing the model to search over a number of vertices exponential in the number of layers. However, we find that as the input graph size increases, the transformer has greater difficulty in learning the task. This difficulty is not resolved even as the number of parameters is increased, suggesting that increasing model scale will not lead to robust search abilities. We also find that performing search in-context (i.e., chain-of-thought) does not resolve this inability to learn to search on larger graphs.

트랜스포머가 그래프 탐색 문제를 학습할 수 있는지에 대한 분석. 조건에 따라 학습할 수 있고 일반화 가능한 알고리즘을 (각 노드에서 접근 가능한 노드들의 집합을 병합하는 방법) 학습할 수 있다고 하네요. 다만 그래프가 커질수록 학습이 어려워진다고. 다음 토큰 예측의 한계를 다룬 연구에서도 비슷한 문제를 태클했었죠. (https://arxiv.org/abs/2403.06963)

<english>
Analysis on whether transformer can learn to solve graph search problem. It is able to learn generalizable algorithm (which merges a set of nodes which is accessible from each nodes) in certain conditions. But it is became harder when the size of graph is larger. A recent study on limitation of next token prediction addressed similar problem. (https://arxiv.org/abs/2403.06963)
</english>

#transformer #mechanistic-interpretation

# Links

[[240311 The pitfalls of next-token prediction.md]]