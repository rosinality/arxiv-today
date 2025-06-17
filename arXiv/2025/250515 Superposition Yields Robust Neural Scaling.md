https://arxiv.org/abs/2505.10465

*Superposition Yields Robust Neural Scaling* (Yizhou liu, Ziming Liu, Jeff Gore)

> The success of today's large language models (LLMs) depends on the observation that larger models perform better. However, the origin of this neural scaling law -- the finding that loss decreases as a power law with model size -- remains unclear. Starting from two empirical principles -- that LLMs represent more things than the model dimensions (widths) they have (i.e., representations are superposed), and that words or concepts in language occur with varying frequencies -- we constructed a toy model to study the loss scaling with model size. We found that when superposition is weak, meaning only the most frequent features are represented without interference, the scaling of loss with model size depends on the underlying feature frequency; if feature frequencies follow a power law, so does the loss. In contrast, under strong superposition, where all features are represented but overlap with each other, the loss becomes inversely proportional to the model dimension across a wide range of feature frequency distributions. This robust scaling behavior is explained geometrically: when many more vectors are packed into a lower dimensional space, the interference (squared overlaps) between vectors scales inversely with that dimension. We then analyzed four families of open-sourced LLMs and found that they exhibit strong superposition and quantitatively match the predictions of our toy model. The Chinchilla scaling law turned out to also agree with our results. We conclude that representation superposition is an important mechanism underlying the observed neural scaling laws. We anticipate that these insights will inspire new training strategies and model architectures to achieve better performance with less computation and fewer parameters.

모델 Scaling에 의한 Loss의 감소가 Power Law를 따르는 이유가 Superposition 때문일 수 있다는 주장. Feature의 분포 자체도 Power Law를 따르지 않을까 싶긴 합니다.

<english>
Suggestion of the reason of loss decrease by model scaling follows power law maybe due to superposition. I think distribution of features would follows power law.
</english>

#mechanistic-interpretation #scaling-law 