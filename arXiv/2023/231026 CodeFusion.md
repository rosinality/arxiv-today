https://arxiv.org/abs/2310.17680

CodeFusion: A Pre-trained Diffusion Model for Code Generation (Mukul Singh, José Cambronero, Sumit Gulwani, Vu Le, Carina Negreanu, Gust Verbruggen)

nl2code diffusion 모델. 자연어 인코더, 임베딩에 대한 denoiser, 임베딩을 토큰으로 전환하는 디코더로 구성되어 있네요. diffusion 모델의 텍스트 생성에 대한 적용에서 길이나 fertility 예측 같은 문제들이 앞으로 어떻게 풀릴지 궁금합니다. (이 논문은 고정 크기로 패딩하는 방식입니다.)

그런데 diffusion 모델 자체보다도 논문에서 gpt-3.5-turbo를 20B라고 적어놓아서 그게 더 화제가 되고 있네요. 오타다, 실제 유출이다 등등의 이야기가 나오고 있는데...과연 진실은?

#ddpm #non-autoregressive 