https://arxiv.org/abs/2310.03734

Leveraging Unpaired Data for Vision-Language Generative Models via Cycle Consistency (Tianhong Li, Sangnie Bhardwaj, Yonglong Tian, Han Zhang, Jarred Barber, Dina Katabi, Guillaume Lajoie, Huiwen Chang, Dilip Krishnan)

와 Cycle Consistency! 정말 오랜만에 들어보는 표현 같네요. Image-to-Text와 Text-to-Image 모듈을 학습시키는데, Unpaired Image/Text를 사용하기 위해 CycleGAN 같은 Cycle Consistency를 주입합니다.

1. 기본적으로 I2T와 T2I는 이미지-텍스트 인코더를 공유하고 독립적인 이미지/텍스트 디코더를 사용합니다. 이미지 인코더는 MAE 기반이네요.
2. Text-Image-Text: T2I로 텍스트에서 이미지 생성, 마스킹한 이미지를 I2T에 입력으로 주고 입력 텍스트를 사용해 Loss를 계산합니다.
3. Image-Text-Image: I2T로 이미지에서 텍스트를 생성하고, 마스킹한 이미지와 생성한 텍스트를 사용해 T2I로 마스킹된 부분에 대해 입력 이미지로 Loss를 계산합니다.

Paired 데이터를 사용하는 것과 대비해 비슷한 scalability를 보여주고, 이미지-텍스트 페어의 퀄리티가 낮을 경우를 고려하면 오히려 더 나아질 수도 있다는 결과를 시사하네요. 흥미롭습니다.

#text2img #captioning 