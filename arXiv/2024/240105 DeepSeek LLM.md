https://arxiv.org/abs/2401.02954

DeepSeek LLM: Scaling Open-Source Language Models with Longtermism (DeepSeek-AI: Xiao Bi, Deli Chen, Guanting Chen, Shanhuang Chen, Damai Dai, Chengqi Deng, Honghui Ding, Kai Dong, Qiushi Du, Zhe Fu, Huazuo Gao, Kaige Gao, Wenjun Gao, Ruiqi Ge, Kang Guan, Daya Guo, Jianzhong Guo, Guangbo Hao, Zhewen Hao, Ying He, Wenjie Hu, Panpan Huang, Erhang Li, Guowei Li, Jiashi Li, Yao Li, Y.K. Li, Wenfeng Liang, Fangyun Lin, A.X. Liu, Bo Liu, Wen Liu, Xiaodong Liu, Xin Liu, Yiyuan Liu, Haoyu Lu, Shanghao Lu, Fuli Luo, Shirong Ma, Xiaotao Nie, Tian Pei, Yishi Piao, Junjie Qiu, Hui Qu, Tongzheng Ren, Zehui Ren, Chong Ruan, Zhangli Sha, Zhihong Shao, Junxiao Song, Xuecheng Su, Jingxiang Sun, Yaofeng Sun, Minghui Tang, Bingxuan Wang, Peiyi Wang, Shiyu Wang, Yaohui Wang, Yongji Wang, Tong Wu, Y. Wu, Xin Xie, Zhenda Xie, Ziwei Xie, Yiliang Xiong, Hanwei Xu, R.X. Xu, Yanhong Xu, Dejian Yang, Yuxiang You, Shuiping Yu, Xingkai Yu, B. Zhang, Haowei Zhang, Lecong Zhang, Liyue Zhang, Mingchuan Zhang, Minghua Zhang, Wentao Zhang, Yichao Zhang, Chenggang Zhao, Yao Zhao, Shangyan Zhou, Shunfeng Zhou, Qihao Zhu, Yuheng Zou)

DeepSeek의 LLM 리포트. 굉장히 흥미롭네요. 주로 눈에 띄는 것은 Scaling 실험들입니다. 파라미터를 모델 FLOPs로 교체한 다음 배치 크기와 LR에 대한 Scaling, Optimal Model/Data 크기, 그리고 다른 데이터셋이 달라졌을 때에 대한 계수의 변화를 봤습니다. 데이터 퀄리티가 높아질수록 모델 크기에 대한 계수가 높아지고 데이터에 대한 계수가 낮아진다는 것 같은 부분도 흥미로운 포인트인 듯 싶네요. 사실 Chinchilla Scaling의 데이터셋에 대한 요인이 고려에서 배제되어 있었던 감이 있죠.

요즘 중국쪽 LLM들이 그렇듯 Alignment 튜닝에 대한 결과들도 있습니다. 요즘 인기 있는 방식인 Instruction 데이터를 프리트레이닝에 추가하는 것에 대해 언급한 부분도 눈에 띄네요. 학습 세팅 변경의 편의성을 위해 Cosine LR 대신 MultiStep LR을 썼다는 것 같은 디테일도 재미있습니다.

결론 부분의 언급을 보면 MoE 실험도 한 것 같군요. 리포트를 공개할 예정이라고 합니다. 추가로 코드 모델에 대해서도 언급하고 있는데 DeepSeek Coder는 Dependency에 따라 코드를 정렬하는 접근을 사용한 게 특징적이었죠. 이쪽도 기대가 되네요.

#llm #pretraining 