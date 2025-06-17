https://arxiv.org/abs/2407.07726

*PaliGemma: A versatile 3B VLM for transfer* (Lucas Beyer, Andreas Steiner, André Susano Pinto, Alexander Kolesnikov, Xiao Wang, Daniel Salz, Maxim Neumann, Ibrahim Alabdulmohsin, Michael Tschannen, Emanuele Bugliarello, Thomas Unterthiner, Daniel Keysers, Skanda Koppula, Fangyu Liu, Adam Grycner, Alexey Gritsenko, Neil Houlsby, Manoj Kumar, Keran Rong, Julian Eisenschlos, Rishabh Kabra, Matthias Bauer, Matko Bošnjak, Xi Chen, Matthias Minderer, Paul Voigtlaender, Ioana Bica, Ivana Balazevic, Joan Puigcerver, Pinelopi Papalampidi, Olivier Henaff, Xi Xiong, Radu Soricut, Jeremiah Harmsen, Xiaohua Zhai)

> PaliGemma is an open Vision-Language Model (VLM) that is based on the SigLIP-So400m vision encoder and the Gemma-2B language model. It is trained to be a versatile and broadly knowledgeable base model that is effective to transfer. It achieves strong performance on a wide variety of open-world tasks. We evaluate PaliGemma on almost 40 diverse tasks including standard VLM benchmarks, but also more specialized tasks such as remote-sensing and segmentation.

PaliGemma의 테크니컬 리포트가 나왔군요. SigLip 400M + Gemma 2B의 조합입니다.

이미지와 Prefix에 대해 Bidirectional Attention을 사용한 PrefixLM, 인코더도 같이 학습하되 인코더에 대해서는 더 긴 LR Warmup을 사용, 크롭 없이 이미지 해상도 확장 등이 특징이군요. 그리고 여전히 Inv-Sqrt Infinite LR 스케줄을 쓰고 있네요.

#vision-language 