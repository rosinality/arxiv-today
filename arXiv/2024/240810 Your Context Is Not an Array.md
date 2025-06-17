https://arxiv.org/abs/2408.05506

*Your Context Is Not an Array: Unveiling Random Access Limitations in Transformers* (MohammadReza Ebrahimi, Sunny Panchal, Roland Memisevic)

> Despite their recent successes, Transformer-based large language models show surprising failure modes. A well-known example of such failure modes is their inability to length-generalize: solving problem instances at inference time that are longer than those seen during training. In this work, we further explore the root cause of this failure by performing a detailed analysis of model behaviors on the simple parity task. Our analysis suggests that length generalization failures are intricately related to a model's inability to perform random memory accesses within its context window. We present supporting evidence for this hypothesis by demonstrating the effectiveness of methodologies that circumvent the need for indexing or that enable random token access indirectly, through content-based addressing. We further show where and how the failure to perform random memory access manifests through attention map visualizations.

Transformer의 Length Extrapolation 문제가 Attention이 Content 기반 Addressing은 가능하지만 Index/Location 기반 Addressing은 어렵다는 점에서 기인한다는 아이디어. 따라서 Location 기반 Addressing을 쉽게 할 수 있도록 토큰을 끼워넣거나 시퀀스를 재배치하면 Length Extrapolation이 발생할 수 있다고 합니다.

Location 기반 Addressing이라는 표현이 말해주듯 Length Extrapolation이 결국 Positional Encoding과 관련된 문제라는 것과 연결되는 것 같네요. Location 기반 Addressing이라고 하니 Neural Turing Machine도 떠오르는군요.

#transformer #positional-encoding #extrapolation 