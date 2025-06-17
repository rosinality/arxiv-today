https://arxiv.org/abs/2503.16057

*Expert Race: A Flexible Routing Strategy for Scaling Diffusion Transformer with Mixture of Experts* (Yike Yuan, Ziyu Wang, Zihao Huang, Defa Zhu, Xun Zhou, Jingyi Yu, Qiyang Min)

> Diffusion models have emerged as mainstream framework in visual generation. Building upon this success, the integration of Mixture of Experts (MoE) methods has shown promise in enhancing model scalability and performance. In this paper, we introduce Race-DiT, a novel MoE model for diffusion transformers with a flexible routing strategy, Expert Race. By allowing tokens and experts to compete together and select the top candidates, the model learns to dynamically assign experts to critical tokens. Additionally, we propose per-layer regularization to address challenges in shallow layer learning, and router similarity loss to prevent mode collapse, ensuring better expert utilization. Extensive experiments on ImageNet validate the effectiveness of our approach, showcasing significant performance gains while promising scaling properties.

각 토큰 당 k개 Expert라는 제약을 풀고 배치 전체에 대해 Expert를 할당하는 방법이네요. 이런 방법은 학습과 추론 시점에 차이가 발생한다는 것이 문제이긴 하죠. (이쪽도 그에 대해 대응하려고 시도했습니다.) 그렇지만 동일한 k개 Expert 사용이라는 제약을 푸는 것은 흥미로운 방향이네요. 최적화가 더 까다로워지겠습니다만.

<english>
Relieving the restriction of expert assignment of k experts per tokens by assigning experts over batch. The problem of these kind methods is there would be gap between training and inference (this paper also tried to resolve it). But I think reliving limitation of using uniform k experts is interesting research direction. It would make optimization harder, though.
</english>

#moe 