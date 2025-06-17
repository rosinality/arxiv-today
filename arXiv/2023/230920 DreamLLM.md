https://arxiv.org/abs/2309.11499

DreamLLM: Synergistic Multimodal Comprehension and Creation (Runpei Dong, Chunrui Han, Yuang Peng, Zekun Qi, Zheng Ge, Jinrong Yang, Liang Zhao, Jianjian Sun, Hongyu Zhou, Haoran Wei, Xiangwen Kong, Xiangyu Zhang, Kaisheng Ma, Li Yi)

image-text interleaved generation. clip 임베딩에 정렬한다거나 하는 대신, 이미지 생성 쿼리 토큰에 대해서 나온 임베딩을 projection 해서 diffusion을 사용해 loss를 계산해 학습시키고, 타겟 이미지를 다시 projection해서 lm의 입력으로 주는 흐름이군요.

#vision-language #multimodal_generation 