https://arxiv.org/abs/2410.21273

*On Inductive Biases That Enable Generalization of Diffusion Transformers* (Jie An, De Wang, Pengsheng Guo, Jiebo Luo, Alexander Schwing)

> Recent work studying the generalization of diffusion models with UNet-based denoisers reveals inductive biases that can be expressed via geometry-adaptive harmonic bases. However, in practice, more recent denoising networks are often based on transformers, e.g., the diffusion transformer (DiT). This raises the question: do transformer-based denoising networks exhibit inductive biases that can also be expressed via geometry-adaptive harmonic bases? To our surprise, we find that this is not the case. This discrepancy motivates our search for the inductive bias that can lead to good generalization in DiT models. Investigating the pivotal attention modules of a DiT, we find that locality of attention maps are closely associated with generalization. To verify this finding, we modify the generalization of a DiT by restricting its attention windows. We inject local attention windows to a DiT and observe an improvement in generalization. Furthermore, we empirically find that both the placement and the effective attention size of these local attention windows are crucial factors. Experimental results on the CelebA, ImageNet, and LSUN datasets show that strengthening the inductive bias of a DiT can improve both generalization and generation quality when less training data is available. Source code will be released publicly upon paper publication. Project page: dit-generalization.github.io/.

UNet에서는 Inductive bias로 인해 진동수에 따라 정렬된 기하학적 패턴이 나타나지만 DiT에서는 잘 나타나지 않는다는 분석. 따라서 Local Attention으로 Inductive bias를 주입하면 DiT의 일반화 성능이 개선된다는 결과. ViT의 초창기에 많이 했던 작업이죠. 요즘은 Inductive bias를 주입한다고 하면 다들 꺼릴 것 같긴 합니다만.

<english>
UNet shows geometric pattern aligned with frequencies due to inductive biases, but it is now occuring in DiT. So we can improve generalization of DiT by injecting inductive bias using local attention. It is a line of work that occured in the early era of ViT. I think many people would wary of injecting inductive bias in these days, though.
</english>

#diffusion #transformer #inductive-bias
