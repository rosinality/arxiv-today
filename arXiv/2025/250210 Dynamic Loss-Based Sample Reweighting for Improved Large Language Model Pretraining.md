https://arxiv.org/abs/2502.06733

*Dynamic Loss-Based Sample Reweighting for Improved Large Language Model Pretraining* (Daouda Sow, Herbert Woisetschläger, Saikiran Bulusu, Shiqiang Wang, Hans-Arno Jacobsen, Yingbin Liang)

> Pretraining large language models (LLMs) on vast and heterogeneous datasets is crucial for achieving state-of-the-art performance across diverse downstream tasks. However, current training paradigms treat all samples equally, overlooking the importance or relevance of individual samples throughout the training process. Existing reweighting strategies, which primarily focus on group-level data importance, fail to leverage fine-grained instance-level information and do not adapt dynamically to individual sample importance as training progresses. In this paper, we introduce novel algorithms for dynamic, instance-level data reweighting aimed at improving both the efficiency and effectiveness of LLM pretraining. Our methods adjust the weight of each training sample based on its loss value in an online fashion, allowing the model to dynamically focus on more informative or important samples at the current training stage. In particular, our framework allows us to systematically devise reweighting strategies deprioritizing redundant or uninformative data, which we find tend to work best. Furthermore, we develop a new theoretical framework for analyzing the impact of loss-based reweighting on the convergence of gradient-based optimization, providing the first formal characterization of how these strategies affect convergence bounds. We empirically validate our approach across a spectrum of tasks, from pretraining 7B and 1.4B parameter LLMs to smaller-scale language models and linear regression problems, demonstrating that our loss-based reweighting approach can lead to faster convergence and significantly improved performance.

Loss Reweighting을 통한 LM 학습 개선. Learnability (https://arxiv.org/abs/2310.15389, https://arxiv.org/abs/2404.07965) 계통의 연구들이 생각나는데 학습 중인 모델 자체의 Loss 통계만으로 잘 작동할지 궁금하네요.

<english>
Improving LM training using loss reweighting. It reminds me learnability related researches (https://arxiv.org/abs/2310.15389, https://arxiv.org/abs/2404.07965) but I wonder it would work only with statistics of loss of the model in training.
</english>

#pretraining

# Links

[[240411 Rho-1.md]]