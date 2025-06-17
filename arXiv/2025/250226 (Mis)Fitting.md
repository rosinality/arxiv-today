https://arxiv.org/abs/2502.18969

*(Mis)Fitting: A Survey of Scaling Laws* (Margaret Li, Sneha Kudugunta, Luke Zettlemoyer)

> Modern foundation models rely heavily on using scaling laws to guide crucial training decisions. Researchers often extrapolate the optimal architecture and hyper parameters settings from smaller training runs by describing the relationship between, loss, or task performance, and scale. All components of this process vary, from the specific equation being fit, to the training setup, to the optimization method. Each of these factors may affect the fitted law, and therefore, the conclusions of a given study. We discuss discrepancies in the conclusions that several prior works reach, on questions such as the optimal token to parameter ratio. We augment this discussion with our own analysis of the critical impact that changes in specific details may effect in a scaling study, and the resulting altered conclusions. Additionally, we survey over 50 papers that study scaling trends: while 45 of these papers quantify these trends using a power law, most under-report crucial details needed to reproduce their findings. To mitigate this, we we propose a checklist for authors to consider while contributing to scaling law research.

기존 Scaling Law 연구들에 대한 분석과 실험 결과. 주로 Chinchilla의 Parameteric Loss를 다룹니다. 결론적으로는 제대로 하기 어렵다는 이야기를 합니다.

여기서 제안하는 것 중에 파라미터의 수에 주의하라는 것이 중요한 포인트라고 생각합니다. 요즘 Scaling Law들은 상당히 많은 파라미터를 추정하는 경우가 있죠. 그러나 파라미터 다섯 개면 코끼리가 코를 흔들게 할 수 있다는 걸 기억해야 합니다.

<english>
Analysis on previous scaling law researches and experiment results. Mainly this paper deals with parameteric loss from Chinchilla. As conclusion, they say that it is hard to do correct estimation.

I think we should be more cautious about the number of parameters in scaling law is important point. Recent scaling often incorporates and estimates many parameters. But we should always remember we can wiggle trunk of the elephant with five parameters.
</english>

#scaling-law 