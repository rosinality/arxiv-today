https://arxiv.org/abs/2407.09087

*On the Role of Discrete Tokenization in Visual Representation Learning* (Tianqi Du, Yifei Wang, Yisen Wang)

> In the realm of self-supervised learning (SSL), masked image modeling (MIM) has gained popularity alongside contrastive learning methods. MIM involves reconstructing masked regions of input images using their unmasked portions. A notable subset of MIM methodologies employs discrete tokens as the reconstruction target, but the theoretical underpinnings of this choice remain underexplored. In this paper, we explore the role of these discrete tokens, aiming to unravel their benefits and limitations. Building upon the connection between MIM and contrastive learning, we provide a comprehensive theoretical understanding on how discrete tokenization affects the model's generalization capabilities. Furthermore, we propose a novel metric named TCAS, which is specifically designed to assess the effectiveness of discrete tokens within the MIM framework. Inspired by this metric, we contribute an innovative tokenizer design and propose a corresponding MIM method named ClusterMIM. It demonstrates superior performance on a variety of benchmark datasets and ViT backbones. Code is available at https://github.com/PKU-ML/ClusterMIM.

이미지 Discrete Tokenizer에 대한 연구. 이미지 분류 문제 같은 것을 고려할 때 서로 다른 클래스의 이미지에 해당하는 패치가 같은 토큰으로 묶이는 것이 문제가 될 가능성을 생각합니다. 그래서 패치의 픽셀이나 DINO Feature에 대해 K-Means 클러스터링을 사용해 토큰을 만드는 방법을 생각했네요. 

얼마 전 CLIP으로 비슷한 접근을 시도했던 연구가 생각나네요. (https://arxiv.org/abs/2406.11837) 사실 Discrete Tokenizer는 생성, 특히 정보 분량이 그리 높지 않은 이미지를 생성하기 위한 것이 타겟인 방법이라 이미지 인식과는 불협화음이 계속 발생하는 것 같습니다. Continuous Token을 생성하는 방향으로 접근하는 것이 낫지 않을까 하는 생각은 있네요. (물론 이쪽은 이미지 인식이 타겟인 방법이라 이미지 생성에서 불협화음을 내겠죠.)

#vq

# Links

[[240617 Scaling the Codebook Size of VQGAN to 100,000 with a Utilization Rate of 99%.md]]