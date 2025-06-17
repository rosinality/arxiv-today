https://arxiv.org/abs/2311.10089

Emu Edit: Precise Image Editing via Recognition and Generation Tasks (Shelly Sheynin, Adam Polyak, Uriel Singer, Yuval Kirstain, Amit Zohar, Oron Ashual, Devi Parikh, Yaniv Taigman)

이미지 편집 모델. 일단 다양한 CV 과제나 편집 과제를 준비합니다. instruction은 Llama 2로 생성하고, instruction에 상응하는 이미지 페어는 이미지 편집 모델을 사용해서 생성합니다. 편집이나 과제에 따라서 다른데 여기서 중요하게 언급하는 것 중 하나는 특정 영역만 편집해야 하는 과제네요. 이런 경우에 대해 생성한 페어의 정확도를 높이기 위해 마스크를 적용했습니다. 이 마스크는 또한 DINO와 SAM으로 만들어지고요.

이렇게 구축한 데이터셋을 과제 임베딩과 같이 학습시킵니다. 과제 임베딩을 쓴다는 것도 포인트인데, 반대로 few shot으로 새로운 과제에 대해 임베딩을 학습해서 사용할 수 있다고 하네요.

#image_editing 