https://arxiv.org/abs/2311.17921

Do text-free diffusion models learn discriminative visual representations? (Soumik Mukhopadhyay, Matthew Gwilliam, Yosuke Yamaguchi, Vatsal Agarwal, Namitha Padmanabhan, Archana Swaminathan, Tianyi Zhou, Abhinav Shrivastava)

Diffusion 모델에서 representation을 추출하기. diffusion 모델 특성상 어떤 레이어에서, 어떤 스텝에서 representation을 가져올 것인지가 문제가 되는 군요. 그리고 이걸 골라오더라도 그냥 linear probing으로는 충분하지 않고 그 위에 트랜스포머 레이어를 올려야 성능이 나오네요. 여기에 더해 여러 블럭과 스텝의 feature 위에 트랜스포머를 올리거나, upsampling block의 feature를 downsampling block 쪽으로 피드백하는 구조 등을 설계해 테스트했습니다.

사실 feature 위에 올리는 게 많을 수록 헤드가 해준 것이라고 할 수도 있긴 합니다. 그렇지만 최소한 중요한 정보의 손실은 없었다고 할 수 있겠군요.

#diffusion 