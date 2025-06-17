https://arxiv.org/abs/2410.12781

*Long-LRM: Long-sequence Large Reconstruction Model for Wide-coverage Gaussian Splats* (Chen Ziwen, Hao Tan, Kai Zhang, Sai Bi, Fujun Luan, Yicong Hong, Li Fuxin, Zexiang Xu)

> We propose Long-LRM, a generalizable 3D Gaussian reconstruction model that is capable of reconstructing a large scene from a long sequence of input images. Specifically, our model can process 32 source images at 960x540 resolution within only 1.3 seconds on a single A100 80G GPU. Our architecture features a mixture of the recent Mamba2 blocks and the classical transformer blocks which allowed many more tokens to be processed than prior work, enhanced by efficient token merging and Gaussian pruning steps that balance between quality and efficiency. Unlike previous feed-forward models that are limited to processing 1~4 input images and can only reconstruct a small portion of a large scene, Long-LRM reconstructs the entire scene in a single feed-forward step. On large-scale scene datasets such as DL3DV-140 and Tanks and Temples, our method achieves performance comparable to optimization-based approaches while being two orders of magnitude more efficient. Project page: https://arthurhero.github.io/projects/llrm

https://arthurhero.github.io/projects/llrm/

Long Context가 자연스러워지니 Novel View Synthesis 같은 문제에 대해서도 단순하게 이미지를 연결해버리는 접근이 가능하네요.

<english>
As dealing with long context became natural, it became possible to just concatenate multiple images as an input for problems like novel view synthesis
</english>

#long-context #novel-view-synthesis
