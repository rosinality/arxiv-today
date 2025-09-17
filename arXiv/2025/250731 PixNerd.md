https://arxiv.org/abs/2507.23268

*PixNerd: Pixel Neural Field Diffusion* (Shuai Wang, Ziteng Gao, Chenhui Zhu, Weilin Huang, Limin Wang)

> The current success of diffusion transformers heavily depends on the compressed latent space shaped by the pre-trained variational autoencoder(VAE). However, this two-stage training paradigm inevitably introduces accumulated errors and decoding artifacts. To address the aforementioned problems, researchers return to pixel space at the cost of complicated cascade pipelines and increased token complexity. In contrast to their efforts, we propose to model the patch-wise decoding with neural field and present a single-scale, single-stage, efficient, end-to-end solution, coined as pixel neural field diffusion~(PixelNerd). Thanks to the efficient neural field representation in PixNerd, we directly achieved 2.15 FID on ImageNet $256\times256$ and 2.84 FID on ImageNet $512\times512$ without any complex cascade pipeline or VAE. We also extend our PixNerd framework to text-to-image applications. Our PixNerd-XXL/16 achieved a competitive 0.73 overall score on the GenEval benchmark and 80.9 overall score on the DPG benchmark.

#diffusion 