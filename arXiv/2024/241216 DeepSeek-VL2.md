https://github.com/deepseek-ai/DeepSeek-VL2/blob/main/DeepSeek_VL2_paper.pdf

*DeepSeek-VL2: Mixture-of-Experts Vision-Language Models for Advanced Multimodal Understanding* (Zhiyu Wu, Xiaokang Chen, Zizheng Pan, Xingchao Liu, Wen Liu, Damai Dai, Huazuo Gao, Yiyang Ma, Chengyue Wu, Bingxuan Wang, Zhenda Xie, Yu Wu, Kai Hu, Jiawei Wang, Yaofeng Sun, Yukun Li, Yishi Piao, Kang Guan, Aixin Liu, Xin Xie, Yuxiang You, Kai Dong, Xingkai Yu, Haowei Zhang, Liang Zhao, Yisong Wang, Chong Ruan)

> We present DeepSeek-VL2, an advanced series of large Mixture-of-Experts (MoE) Vision- Language Models that significantly improves upon its predecessor, DeepSeek-VL, through two key major upgrades. For the vision component, we incorporate a dynamic tiling vision encoding strategy designed for processing high-resolution images with different aspect ratios. For the language component, we leverage DeepSeekMoE models with the Multi-head Latent Attention mechanism, which compresses Key-Value cache into latent vectors, to enable efficient inference and high throughput. Trained on an improved vision-language dataset, DeepSeek-VL2 demon- strates superior capabilities across various tasks, including but not limited to visual question answering, optical character recognition, document/table/chart understanding, and visual grounding. Our model series is composed of three variants: DeepSeek-VL2-Tiny, DeepSeek-VL2- Small and DeepSeek-VL2, with 1.0B, 2.8B and 4.5B activated parameters respectively. DeepSeek- VL2 achieves competitive or state-of-the-art performance with similar or fewer activated param- eters compared to existing open-source dense and MoE-based models. Codes and pre-trained models are publicly accessible at https://github.com/deepseek-ai/DeepSeek-VL2.

DeepSeek의 Vision Language 모델이 새로 나왔군요. 아키텍처는 DeepSeek 스타일의 MoE + MLA인데 Aux-loss Free Load Balancing을 (https://arxiv.org/abs/2408.15664) 사용했군요. 흥미로운 방법이라고 생각했는데 DeepSeek 내부에서도 신뢰하고 있는 모양입니다.

데이터셋도 구성을 꽤 바꿨고 Grounding 같은 과제를 추가하기도 했네요. 다만 생각보다 오픈소스 데이터를 꽤 사용하는 편이군요.

<english>
New vision language model from DeepSeek. Architecture is DeepSeek style MoE + MLA, but applied aux-loss free load balancing (https://arxiv.org/abs/2408.15664). I thought it is interesting method, and it seems like that DeepSeek also found it useful internally.

Composition of dataset is changed a lot, and tasks like grounding is added. But they use opensource dataset more than I thought.
</english>

#vision-language #moe 