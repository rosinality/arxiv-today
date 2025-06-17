https://arxiv.org/abs/2503.04715

*Predictable Scale: Part I -- Optimal Hyperparameter Scaling Law in Large Language Model Pretraining* (Houyi Li, Wenzheng Zheng, Jingcheng Hu, Qiufeng Wang, Hanshan Zhang, Zili Wang, Yangshijie Xu, Shuigeng Zhou, Xiangyu Zhang, Daxin Jiang)

> The impressive capabilities of Large Language Models (LLMs) across diverse tasks are now well-established, yet their effective deployment necessitates careful hyperparameter optimization. Through extensive empirical studies involving grid searches across diverse configurations, we discover universal scaling laws governing these hyperparameters: optimal learning rate follows a power-law relationship with both model parameters and data sizes, while optimal batch size scales primarily with data sizes. Our analysis reveals a convex optimization landscape for hyperparameters under fixed models and data size conditions. This convexity implies an optimal hyperparameter plateau. We contribute a universal, plug-and-play optimal hyperparameter tool for the community. Its estimated values on the test set are merely 0.07\% away from the globally optimal LLM performance found via an exhaustive search. These laws demonstrate remarkable robustness across variations in model sparsity, training data distribution, and model shape. To our best known, this is the first work that unifies different model shapes and structures, such as Mixture-of-Experts models and dense transformers, as well as establishes optimal hyperparameter scaling laws across diverse data distributions. This exhaustive optimization process demands substantial computational resources, utilizing nearly one million NVIDIA H800 GPU hours to train 3,700 LLMs of varying sizes and hyperparameters from scratch and consuming approximately 100 trillion tokens in total. To facilitate reproducibility and further research, we will progressively release all loss measurements and model checkpoints through our designated repository https://step-law.github.io/

Hyperparameter Scaling Law. LR은 모델 크기와 학습 데이터의 양에, 배치 크기는 학습 데이터의 양에 의해 결정되는군요. 그리고 이 결과는 모델의 깊이나 너비 등의 차이, MoE에 대한 Sparsity, 그리고 데이터의 차이에 대해 큰 영향이 없었다고 합니다. 굉장한 결과네요.

그런데 파트 2는 뭘까요?

<english>
Hyperparameter scaling law. LR depends on model and training data sizes, and batch sizes solely determined by training data sizes. And this result does not affected very much by model width or depths, sparsity due to MoE, and differences in training data compositions. It is really great results.

By the way, what will be part 2?
</english>

#scaling-law #hyperparameter 