https://arxiv.org/abs/2410.20280

*MarDini: Masked Autoregressive Diffusion for Video Generation at Scale* (Haozhe Liu, Shikun Liu, Zijian Zhou, Mengmeng Xu, Yanping Xie, Xiao Han, Juan C. Pérez, Ding Liu, Kumara Kahatapitiya, Menglin Jia, Jui-Chieh Wu, Sen He, Tao Xiang, Jürgen Schmidhuber, Juan-Manuel Pérez-Rúa)

> We introduce MarDini, a new family of video diffusion models that integrate the advantages of masked auto-regression (MAR) into a unified diffusion model (DM) framework. Here, MAR handles temporal planning, while DM focuses on spatial generation in an asymmetric network design: i) a MAR-based planning model containing most of the parameters generates planning signals for each masked frame using low-resolution input; ii) a lightweight generation model uses these signals to produce high-resolution frames via diffusion de-noising. MarDini's MAR enables video generation conditioned on any number of masked frames at any frame positions: a single model can handle video interpolation (e.g., masking middle frames), image-to-video generation (e.g., masking from the second frame onward), and video expansion (e.g., masking half the frames). The efficient design allocates most of the computational resources to the low-resolution planning model, making computationally expensive but important spatio-temporal attention feasible at scale. MarDini sets a new state-of-the-art for video interpolation; meanwhile, within few inference steps, it efficiently generates videos on par with those of much more expensive advanced image-to-video models.

저해상도 비디오 시퀀스에 대한 Masked Autoregression과 고해상도 시퀀스에 대한 Denoising Diffusion의 결합으로 비디오 생성 모델을 구성.

<english>
Video generation model that combines masked autoregressive model on low resolution video sequences and denoising diffusion model on high resolution sequences.
</english>

#video-generation #non-autoregressive #diffusion 