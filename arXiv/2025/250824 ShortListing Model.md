https://arxiv.org/abs/2508.17345

*ShortListing Model: A Streamlined SimplexDiffusion for Discrete Variable Generation* (Yuxuan Song, Zhe Zhang, Yu Pei, Jingjing Gong, Qiying Yu, Zheng Zhang, Mingxuan Wang, Hao Zhou, Jingjing Liu, Wei-Ying Ma)

> Generative modeling of discrete variables is challenging yet crucial for applications in natural language processing and biological sequence design. We introduce the Shortlisting Model (SLM), a novel simplex-based diffusion model inspired by progressive candidate pruning. SLM operates on simplex centroids, reducing generation complexity and enhancing scalability. Additionally, SLM incorporates a flexible implementation of classifier-free guidance, enhancing unconditional generation performance. Extensive experiments on DNA promoter and enhancer design, protein design, character-level and large-vocabulary language modeling demonstrate the competitive performance and strong potential of SLM. Our code can be found at https://github.com/GenSI-THUAIR/SLM

Simplex에 대한 Diffusion. 후보군들을 단일한 하나의 후보로 줄여나가는 프로세스를 사용.

Diffusion over simplexes which is based on a process that prunes all-ones candidate vectors into one-hot.

#diffusion #lm 