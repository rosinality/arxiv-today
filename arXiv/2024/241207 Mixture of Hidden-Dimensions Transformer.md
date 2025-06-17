https://arxiv.org/abs/2412.05644

*Mixture of Hidden-Dimensions Transformer* (Yilong Chen, Junyuan Shang, Zhengyu Zhang, Jiawei Sheng, Tingwen Liu, Shuohuan Wang, Yu Sun, Hua Wu, Haifeng Wang)

> Transformer models encounter challenges in scaling hidden dimensions efficiently, as uniformly increasing them inflates computational and memory costs while failing to emphasize the most relevant features for each token. For further understanding, we study hidden dimension sparsity and observe that trained Transformers utilize only a small fraction of token dimensions, revealing an "activation flow" pattern. Notably, there are shared sub-dimensions with sustained activation across multiple consecutive tokens and specialized sub-dimensions uniquely activated for each token. To better model token-relevant sub-dimensions, we propose MoHD (Mixture of Hidden Dimensions), a sparse conditional activation architecture. Particularly, MoHD employs shared sub-dimensions for common token features and a routing mechanism to dynamically activate specialized sub-dimensions. To mitigate potential information loss from sparsity, we design activation scaling and group fusion mechanisms to preserve activation flow. In this way, MoHD expands hidden dimensions with negligible increases in computation or parameters, efficient training and inference while maintaining performance. Evaluations across 10 NLP tasks show that MoHD surpasses Vanilla Transformers in parameter efficiency and task performance. It achieves 1.7% higher performance with 50% fewer activation parameters and 3.7% higher performance with a 3x parameter expansion at constant activation cost. MOHD offers a new perspective for scaling the model, showcasing the potential of hidden dimension sparsity to boost efficiency

각 레이어에서 임베딩의 Hidden Dimension의 일부만을 사용하도록 하는 모델. 마치 DeepSeekMoE처럼 모든 토큰에 대해 사용되는 Shared Dimension과 토큰에 따라 결정되는 Specialized Dimension을 분리했습니다.

<english>
A model that only uses a part of embedding hidden dimensions for each layer. Like DeepSeekMoE they separated shared dimension that all token uses and specialized dimensions assigned differently for each tokens.
</english>

#moe #sparsity 