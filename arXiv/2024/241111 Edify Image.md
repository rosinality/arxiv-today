https://arxiv.org/abs/2411.07126

*Edify Image: High-Quality Image Generation with Pixel Space Laplacian Diffusion Models* (NVIDIA: Yuval Atzmon, Maciej Bala, Yogesh Balaji, Tiffany Cai, Yin Cui, Jiaojiao Fan, Yunhao Ge, Siddharth Gururani, Jacob Huffman, Ronald Isaac, Pooya Jannaty, Tero Karras, Grace Lam, J. P. Lewis, Aaron Licata, Yen-Chen Lin, Ming-Yu Liu, Qianli Ma, Arun Mallya, Ashlee Martino-Tarr, Doug Mendez, Seungjun Nah, Chris Pruett, Fitsum Reda, Jiaming Song, Ting-Chun Wang, Fangyin Wei, Xiaohui Zeng, Yu Zeng, Qinsheng Zhang)

> We introduce Edify Image, a family of diffusion models capable of generating photorealistic image content with pixel-perfect accuracy. Edify Image utilizes cascaded pixel-space diffusion models trained using a novel Laplacian diffusion process, in which image signals at different frequency bands are attenuated at varying rates. Edify Image supports a wide range of applications, including text-to-image synthesis, 4K upsampling, ControlNets, 360 HDR panorama generation, and finetuning for image customization.

와 라플라시안 피라미드! 라플라시안 피라미드로 분해된 이미지들에 대한 Diffusion Process의 합으로 Diffusion Process를 구성했군요. 실제 구현에서는 웨이블릿 공간에서 작동하도록 했습니다.

<english>
Wow laplacian pyramid! Define overall diffusion process as a sum of diffusion process on images decomposed by laplacian pyramid. Also, in actual implementations model is working on wavelet space.
</english>

#diffusion 