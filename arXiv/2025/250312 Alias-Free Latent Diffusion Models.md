https://arxiv.org/abs/2503.09419

*Alias-Free Latent Diffusion Models:Improving Fractional Shift Equivariance of Diffusion Latent Space* (Yifan Zhou, Zeqi Xiao, Shuai Yang, Xingang Pan)

> Latent Diffusion Models (LDMs) are known to have an unstable generation process, where even small perturbations or shifts in the input noise can lead to significantly different outputs. This hinders their applicability in applications requiring consistent results. In this work, we redesign LDMs to enhance consistency by making them shift-equivariant. While introducing anti-aliasing operations can partially improve shift-equivariance, significant aliasing and inconsistency persist due to the unique challenges in LDMs, including 1) aliasing amplification during VAE training and multiple U-Net inferences, and 2) self-attention modules that inherently lack shift-equivariance. To address these issues, we redesign the attention modules to be shift-equivariant and propose an equivariance loss that effectively suppresses the frequency bandwidth of the features in the continuous domain. The resulting alias-free LDM (AF-LDM) achieves strong shift-equivariance and is also robust to irregular warping. Extensive experiments demonstrate that AF-LDM produces significantly more consistent results than vanilla LDM across various applications, including video editing and image-to-image translation. Code is available at: https://github.com/SingleZombie/AFLDM

구상하고 있었던 주제였는데 결과가 나와버렸군요. Antialiased Latent Diffusion. 모델을 Antialiased 아키텍처로 수정하고 Equivariance Loss를 추가했네요.

<english>
Result of the idea came out which I thinking about recently. Antialiased latent diffusion. The authors revised architecture into antialiased one and added equivariance loss.
</english>

#diffusion 