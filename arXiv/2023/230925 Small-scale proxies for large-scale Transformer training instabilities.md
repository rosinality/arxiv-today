https://arxiv.org/abs/2309.14322

Small-scale proxies for large-scale Transformer training instabilities (Mitchell Wortsman, Peter J. Liu, Lechao Xiao, Katie Everett, Alex Alemi, Ben Adlam, John D. Co-Reyes, Izzeddin Gur, Abhishek Kumar, Roman Novak, Jeffrey Pennington, Jascha Sohl-dickstein, Kelvin Xu, Jaehoon Lee, Justin Gilmer, Simon Kornblith)

트랜스포머의 학습 불안정성과 그 원인으로 지목되는 두 현상(Attention Logit의 증가와 출력 Logit의 발산)을 작은 모델에서도 LR을 높임으로써 재현할 수 있다는 결과. 이 결과를 기반으로 불안정성을 해소하기 위한 방법들을 테스트했군요. 여기서 안정성을 보는 척도는 높은 LR에서의 발산 여부와, LR의 변동에 따른 Loss의 변동 기대값입니다.

1. QK LayerNorm (https://arxiv.org/abs/2302.05442). Attention Logit의 증가와 관련되어 있죠. QK LayerNorm은 모든 모델 규모에서 불안정성을 낮춰줍니다.
2. z-loss (https://arxiv.org/abs/2204.02311). 출력 Logit의 발산과 관련되어 있죠. 안정성을 높여주지만 큰 모델에서는 Weight Decay로 커버가 되는 것 같군요.
3. Warmup. Warmup이 길면 더 안정합니다.
4. Independent Weight Decay. AdamW의 일반적인 구현에서는 업데이트가 LR * Weight Decay로 되어 있죠. 이걸 분리해서 LR 따로 Weight Decay 따로 지정하면 좀 더 안정합니다.
5. 깊은 모델이 넓은 모델보다 불안정합니다. 그렇다고 안정성을 위해 깊이를 희생할 필요는 없지만요.
6. μP (https://arxiv.org/abs/2203.03466). 이거 다들 찍먹해보는 군요. 안정성에는 영향이 없다고 합니다. 그렇지만 어차피 최적 하이퍼파라미터를 찾기 위한 방법이니 안정성을 요구할 문제는 아니긴 하죠.
7. Attention Logit의 불안정성은 ReLU 같은 걸 써도 발생하는 걸로 봐선 Softmax 때문은 아니라고 합니다.
8. LR이 어느 정도일 때 불안정해질 것인지 예측이 가능한가? 아직 증거가 부족하지만 그런 것 같다고 합니다.
9. 한 가지 더. 모델이 클 때 낮은 단계의 레이어에서 그래디언트의 크기가 Adam의 eps보다 작아지면 불안정해질 수 있습니다. eps를 키워서 안정하게 만드는 건 봤는데 eps를 낮춰서 안정성을 높이는 건 여기서 처음 보네요.

Weight의 Norm의 증가를 억제하는 방법은 여러 가지 있겠지만 제가 익숙한 건 AdamP (https://arxiv.org/abs/2006.08217) 같은 접근입니다. QK LayerNorm 등의 도입 없이 이런 수정을 통해 불안정성을 해소할 수 있을지 궁금하네요.

#transformer #stability

# Links

# Links

