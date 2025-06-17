https://arxiv.org/abs/2408.07852

*Training Language Models on the Knowledge Graph: Insights on Hallucinations and Their Detectability* (Jiri Hron, Laura Culp, Gamaleldin Elsayed, Rosanne Liu, Ben Adlam, Maxwell Bileschi, Bernd Bohnet, JD Co-Reyes, Noah Fiedel, C. Daniel Freeman, Izzeddin Gur, Kathleen Kenealy, Jaehoon Lee, Peter J. Liu, Gaurav Mishra, Igor Mordatch, Azade Nova, Roman Novak, Aaron Parisi, Jeffrey Pennington, Alex Rizkowsky, Isabelle Simpson, Hanie Sedghi, Jascha Sohl-dickstein, Kevin Swersky, Sharad Vikram, Tris Warkentin, Lechao Xiao, Kelvin Xu, Jasper Snoek, Simon Kornblith)

> While many capabilities of language models (LMs) improve with increased training budget, the influence of scale on hallucinations is not yet fully understood. Hallucinations come in many forms, and there is no universally accepted definition. We thus focus on studying only those hallucinations where a correct answer appears verbatim in the training set. To fully control the training data content, we construct a knowledge graph (KG)-based dataset, and use it to train a set of increasingly large LMs. We find that for a fixed dataset, larger and longer-trained LMs hallucinate less. However, hallucinating on $\leq5$% of the training data requires an order of magnitude larger model, and thus an order of magnitude more compute, than Hoffmann et al. (2022) reported was optimal. Given this costliness, we study how hallucination detectors depend on scale. While we see detector size improves performance on fixed LM's outputs, we find an inverse relationship between the scale of the LM and the detectability of its hallucinations.

Knowledge Graph에 대해 학습시켜 LLM의 Hallucination에 대한 Scaling 특성을 연구. 더 큰 모델을 데이터에 대해 (Multi Epoch로) 더 오래 학습시킬수록 Hallucination Rate는 감소합니다. 그렇지만 데이터가 커지면 Hallucination Rate는 증가하네요.

Hallucination 탐지의 경우에는 큰 모델이 Hallucination Rate가 낮은 동시에 Hallucination 탐지도 더 어려워지네요.

#hallucination 