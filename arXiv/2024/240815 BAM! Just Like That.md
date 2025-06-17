https://arxiv.org/abs/2408.08274

*BAM! Just Like That: Simple and Efficient Parameter Upcycling for Mixture of Experts* (Qizhen Zhang, Nikolas Gritsch, Dwaraknath Gnaneshwar, Simon Guo, David Cairuz, Bharat Venkitesh, Jakob Foerster, Phil Blunsom, Sebastian Ruder, Ahmet Ustun, Acyr Locatelli)

> The Mixture of Experts (MoE) framework has become a popular architecture for large language models due to its superior performance over dense models. However, training MoEs from scratch in a large-scale regime is prohibitively expensive. Existing methods mitigate this by pre-training multiple dense expert models independently and using them to initialize an MoE. This is done by using experts' feed-forward network (FFN) to initialize the MoE's experts while merging other parameters. However, this method limits the reuse of dense model parameters to only the FFN layers, thereby constraining the advantages when "upcycling" these models into MoEs. We propose BAM (Branch-Attend-Mix), a simple yet effective method that addresses this shortcoming. BAM makes full use of specialized dense models by not only using their FFN to initialize the MoE layers but also leveraging experts' attention parameters fully by initializing them into a soft-variant of Mixture of Attention (MoA) layers. We explore two methods for upcycling attention parameters: 1) initializing separate attention experts from dense models including all attention parameters for the best model performance; and 2) sharing key and value parameters across all experts to facilitate for better inference efficiency. To further improve efficiency, we adopt a parallel attention transformer architecture to MoEs, which allows the attention experts and FFN experts to be computed concurrently. Our experiments on seed models ranging from 590 million to 2 billion parameters demonstrate that BAM surpasses baselines in both perplexity and downstream task performance, within the same computational and data constraints.

Branch-Train-Mix스러운 (https://arxiv.org/abs/2403.07816) 각 도메인에 대해 모델을 학습한 다음 Sparse Upcycling으로 결합하는 방법. 여기서는 FFN 뿐만 아니라 Attention을 결합하는 것이 핵심이네요. 다만 Sparse MoE로 결합하는 것으로는 안 되고 Soft하게 모두 결합해야 한다고 합니다. Mixture of Attention 자체에 대한 연구가 더 필요하지 않을까 하는 생각이 드네요.

#moe

# Links

[[240312 Branch-Train-MiX.md]]