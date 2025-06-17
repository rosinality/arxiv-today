https://arxiv.org/abs/2310.01693

Closing the Curious Case of Neural Text Degeneration (Matthew Finlayson, John Hewitt, Alexander Koller, Swabha Swayamdipta, Ashish Sabharwal)

Nuecleus 샘플링이나 Top-K 샘플링은 어떤 역치를 사용해서 분포의 꼬리를 잘라내는데, 이건 실제 확률이 0이 아닌 토큰들만 남겨놓기 위한 방법이라고 이야기합니다. 그렇지만 역치 하나로 이 문제를 해결하는 건 좀 거친 방법이죠. (실제 확률이 0이 아닌 경우에도 잘려나가거나, 혹은 0인 경우에도 남거나.)

그런데 애초에 이 문제가 왜 생기는 것일까? 여기에서 Softmax Bottleneck (https://arxiv.org/abs/1711.03953) 이 등장합니다. 임베딩 차원이 vocab 수보다 작으니 분포의 low rank 근사일 수밖에 없다는 문제죠. 그러니 실제 확률이 0인 경우에도 0이 아닌 값이 부여되게 됩니다. 이걸 여기서 다시 보네요.

그렇다고 Mixture of Softmaxes를 당장 적용할 수 있는 것은 아니니 어떻게 해야할까. 이 논문에서는 cross entropy를 최소화한다는 모델의 학습 방식에 근거해 모델 출력 분포가 근사하는 분포 중에서 특정 토큰의 확률이 0인 분포가 없다면 그 토큰의 실제 확률은 0이 아닐 것이라고 봅니다.

이 문제를 실제로 풀려면 선형 계획 문제를 풀어야 해서 비싸긴 합니다. 여러 방식으로 문제를 축소시켜도 토큰 당 0.1초 정도가 걸린다고 하네요. 결과에서 아주 뚜렷하게 이점이 보이는 것 같지는 않긴 합니다만...여하간 흥미로운 문제에 대한 지적으로 보입니다.

#lm

# Links

# Links

