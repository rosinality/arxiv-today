https://arxiv.org/abs/2310.19341

Skywork: A More Open Bilingual Foundation Model (Tianwen Wei, Liang Zhao, Lichang Zhang, Bo Zhu, Lijie Wang, Haihua Yang, Biye Li, Cheng Cheng, Weiwei Lü, Rui Hu, Chenxia Li, Liu Yang, Xilin Luo, Xuejie Wu, Lunan Liu, Wenjun Cheng, Peng Cheng, Jianhao Zhang, Xiaoyu Zhang, Lei Lin, Xiaokun Wang, Yutuan Ma, Chuanhai Dong, Yanqi Sun, Yifu Chen, Yongyi Peng, Xiaojuan Liang, Shuicheng Yan, Han Fang, Yahui Zhou)

https://github.com/SkyworkAI/Skywork

13B, 3.2T 토큰 학습의 영어/중국어 bilingual llm이네요. 데이터셋 디테일 등에서 역시 개략적인 정보 밖에 없지만 학습 과정은 좀 재미있네요. 2T 정도 학습시키다가 계획 변경으로 추가 데이터 1T에 학습시키고, STEM 쪽 데이터로 200B를 더 학습 시킨 과정에 대한 이야기가 나와 있습니다.

추가로 GSM8K의 학습 데이터를 다른 모델들이 코퍼스에 넣고 있는 것이 아닌가 하는 분석을 하고 있습니다. 학습 셋과 테스트 셋에 대한 perplexity가 좀 차이가 있는데? 하는 분석이네요. 논문에서도 주장하는 것이지만 이런 벤치마크 오염은 피하는 쪽이 좋지 않을까 싶습니다.

#llm #multilingual #pretraining 