https://arxiv.org/abs/2505.12082

*Model Merging in Pre-training of Large Language Models* (Yunshui Li, Yiyuan Ma, Shen Yan, Chaoyi Zhang, Jing Liu, Jianqiao Lu, Ziwen Xu, Mengzhao Chen, Minrui Wang, Shiyi Zhan, Jin Ma, Xunhao Lai, Yao Luo, Xingyan Bin, Hongbin Ren, Mingji Han, Wenhao Hao, Bairen Yi, LingJun Liu, Bole Ma, Xiaoying Jia, Zhou Xun, Liang Xiang, Yonghui Wu)

> Model merging has emerged as a promising technique for enhancing large language models, though its application in large-scale pre-training remains relatively unexplored. In this paper, we present a comprehensive investigation of model merging techniques during the pre-training process. Through extensive experiments with both dense and Mixture-of-Experts (MoE) architectures ranging from millions to over 100 billion parameters, we demonstrate that merging checkpoints trained with constant learning rates not only achieves significant performance improvements but also enables accurate prediction of annealing behavior. These improvements lead to both more efficient model development and significantly lower training costs. Our detailed ablation studies on merging strategies and hyperparameters provide new insights into the underlying mechanisms while uncovering novel applications. Through comprehensive experimental analysis, we offer the open-source community practical pre-training guidelines for effective model merging.

프리트레이닝에 Averaged SGD를 쓴 실험에 대한 결과군요. 학습 중간에 LR Annealing을 하지 않더라도 Annealing을 한 것과 비슷한 결과가 나온다는 것이 유용한 경우도 있을 것 같습니다. 그리고 파인튜닝의 초기 체크포인트로 쓰기에도 괜찮았다고 하는군요. MoE에 좀 더 잘 맞을 것 같기도 합니다.

<english>
Result on applying averaged SGD on pretraining. There could be useful cases that you can get a LR annealed results during pretraining without actually doing an annealing. The paper also says that it was better for initial checkpoint for finetuning. I think it maybe be better fit with MoE.
</english>

#pretraining #optimizer 