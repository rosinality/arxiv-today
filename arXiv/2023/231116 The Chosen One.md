https://arxiv.org/abs/2311.10093

The Chosen One: Consistent Characters in Text-to-Image Diffusion Models (Omri Avrahami, Amir Hertz, Yael Vinker, Moab Arar, Shlomi Fruchter, Ohad Fried, Daniel Cohen-Or, Dani Lischinski)

일관된 캐릭터로 이미지를 생성하는 방법. 일단 이미지를 여러 장 생성한 다음 DINOv2로 feature를 뽑고 클러스터링합니다. 너무 작은 클러스터는 빼고 나머지 클러스터 중 클러스터 내 원소 사이의 거리가 가장 좁은 클러스터를 고릅니다. 그 다음 이 클러스터 내 이미지로 모델을 튜닝합니다. 그리고 이 과정을 충분히 좁은 클러스터가 나올 때까지 반복합니다. 뭔가 의도와 맞는 클러스터가 잘 걸려야 할 것 같긴 합니다만 샘플들이 꽤 인상적이네요.

#image_generation 