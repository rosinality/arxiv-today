https://github.com/deepseek-ai/DeepSeek-Coder-V2/blob/main/paper.pdf

*DeepSeek-Coder-V2: Breaking the Barrier of Closed-Source Models in Code Intelligence* (Qihao Zhu, Daya Guo, Zhihong Shao, Dejian Yang, Peiyi Wang, Runxin Xu, Y. Wu Yukun Li, Huazuo Gao, Shirong Ma, Wangding Zeng, Xiao Bi, Zihui Gu, Hanwei Xu, Damai Dai Kai Dong, Liyue Zhang, Yishi Piao, Zhibin Gou, Zhenda Xie, Zhewen Hao, Bingxuan Wang Junxiao Song, Deli Chen, Xin Xie, Kang Guan, Yuxiang You, Aixin Liu, Qiushi Du, Wenjun Gao Xuan Lu, Qinyu Chen, Yaohui Wang, Chengqi Deng, Jiashi Li, Chenggang Zhao Chong Ruan, Fuli Luo, Wenfeng Liang)

> We present DeepSeek-Coder-V2, an open-source Mixture-of-Experts (MoE) code language model that achieves performance comparable to GPT4-Turbo in code-specific tasks. Specifically, DeepSeek-Coder-V2 is further pre-trained from an intermediate checkpoint of DeepSeek-V2 with additional 6 trillion tokens. Through this continued pre-training, DeepSeek-Coder-V2 substantially enhances the coding and mathematical reasoning capabilities of DeepSeek-V2, while maintaining comparable performance in general language tasks. Compared to DeepSeek- Coder-33B, DeepSeek-Coder-V2 demonstrates significant advancements in various aspects of code-related tasks, as well as reasoning and general capabilities. Additionally, DeepSeek-Coder- V2 expands its support for programming languages from 86 to 338, while extending the context length from 16K to 128K. In standard benchmark evaluations, DeepSeek-Coder-V2 achieves superior performance compared to closed-source models such as GPT4-Turbo, Claude 3 Opus, and Gemini 1.5 Pro in coding and math benchmarks.

DeepSeek의 코드 모델 V2가 나왔군요. DeepSeek V2의 중간 체크포인트를 기반으로 6T를 추가 학습시켜 10.2T 학습 모델을 구축했습니다. 벤치마크 스코어로는 최고 수준의 코드 모델이라고 할 수 있을 듯 하네요.

일단 GitHub을 털어 1T 토큰을 확보하고 DeepSeekMath (https://arxiv.org/abs/2402.03300) 의 접근을 코드에 적용해 164B의 코드 관련 토큰을 확요했고. 추가로 120B였던 수학 관련 데이터를 221B로 확고했습니다.

RL 과정에서 Reward Modeling도 흥미롭네요. 테스트를 사용한 컴파일러 피드백으로 0-1 피드백을 줄 수 있지만 테스트가 충분하지 않을 수 있으므로 이 피드백도 충분하지는 않다고 판단했습니다. 따라서 컴파일러 피드백의 결과로 Reward Model을 학습시키고 이 Reward Model로 RL을 진행했다고 하네요.

#llm 