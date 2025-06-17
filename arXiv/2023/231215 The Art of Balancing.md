https://arxiv.org/abs/2312.09979

The Art of Balancing: Revolutionizing Mixture of Experts for Maintaining World Knowledge in Language Model Alignment (Shihan Dou, Enyu Zhou, Yan Liu, Songyang Gao, Jun Zhao, Wei Shen, Yuhao Zhou, Zhiheng Xi, Xiao Wang, Xiaoran Fan, Shiliang Pu, Jiang Zhu, Rui Zheng, Tao Gui, Qi Zhang, Xuanjing Huang)

Instruction tuning 데이터를 증가시켜보면 어떤 과제에 대해서는 성능이 향상되는데 지식을 묻는 과제들, Closed Book Question Answering에 대해서는 성능이 떨어진다, 이 문제를 LoRA로 MoE를 구성해 대응하겠다는 아이디어입니다.

구체적인 대응 방법과는 별개로 1. 대규모의 Instruction tuning 데이터는 (요즘 많이 하는 것처럼) 프리트레이닝에 밀어넣는 것이 편리할 수 있다. 2. MoE 모델이 이 문제에 대해 전반적으로 유용할 수 있겠다는 생각이 드네요.

#instruction-tuning #efficient_training #moe