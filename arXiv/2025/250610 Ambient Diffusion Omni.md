https://arxiv.org/abs/2506.10038

*Ambient Diffusion Omni: Training Good Models with Bad Data* (Giannis Daras, Adrian Rodriguez-Munoz, Adam Klivans, Antonio Torralba, Constantinos Daskalakis)

> We show how to use low-quality, synthetic, and out-of-distribution images to improve the quality of a diffusion model. Typically, diffusion models are trained on curated datasets that emerge from highly filtered data pools from the Web and other sources. We show that there is immense value in the lower-quality images that are often discarded. We present Ambient Diffusion Omni, a simple, principled framework to train diffusion models that can extract signal from all available images during training. Our framework exploits two properties of natural images -- spectral power law decay and locality. We first validate our framework by successfully training diffusion models with images synthetically corrupted by Gaussian blur, JPEG compression, and motion blur. We then use our framework to achieve state-of-the-art ImageNet FID, and we show significant improvements in both image quality and diversity for text-to-image generative modeling. The core insight is that noise dampens the initial skew between the desired high-quality distribution and the mixed distribution we actually observe. We provide rigorous theoretical justification for our approach by analyzing the trade-off between learning from biased data versus limited unbiased data across diffusion times.

노이즈 비율이 높은 시점에 저품질 데이터를, 노이즈 비율이 낮은 시점에 OOD 데이터의 크롭을 사용해서 사용 데이터를 증가시킨다는 아이디어.

<english>
The idea of expand data used for training by using low quality data for the time when ratio of noise is high, and crop of OOD data for the time when ratio of noise is low.
</english>

#diffusion 