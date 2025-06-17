https://arxiv.org/abs/2311.17528

HiDiffusion: Unlocking High-Resolution Creativity and Efficiency in Low-Resolution Trained Diffusion Models (Shen Zhang, Zhaowei Chen, Zhenyu Zhao, Zhenyuan Chen, Yao Tang, Yuhao Chen, Wengang Cao, Jiajun Liang)

학습 없이 Diffusion 모델의 해상도 높이기. 얼마 전에 본 Scale Crafter (https://arxiv.org/abs/2310.07702) 가 생각나네요. 첫 레이어에서 Strided conv를 써서 downsampling, 마지막 레이어에서 interpolation으로 upsampling을 하고 blurriness 문제 해결을 위해 샘플링 과정의 초기에만 downsample/upsample을 사용하는 네트워크를 적용합니다.

추가로 속도가 너무 느린 것을 해소하기 위해 self attention을 window self attention으로 교체했네요.

#diffusion 

[[231011 ScaleCrafter]]

# Links

[[231011 ScaleCrafter.md]]