https://arxiv.org/abs/2411.10442

*Enhancing the Reasoning Ability of Multimodal Large Language Models via Mixed Preference Optimization* (Weiyun Wang, Zhe Chen, Wenhai Wang, Yue Cao, Yangzhou Liu, Zhangwei Gao, Jinguo Zhu, Xizhou Zhu, Lewei Lu, Yu Qiao, Jifeng Dai)

> Existing open-source multimodal large language models (MLLMs) generally follow a training process involving pre-training and supervised fine-tuning. However, these models suffer from distribution shifts, which limit their multimodal reasoning, particularly in the Chain-of-Thought (CoT) performance. To address this, we introduce a preference optimization (PO) process to enhance the multimodal reasoning capabilities of MLLMs. Specifically, (1) on the data side, we design an automated preference data construction pipeline to create MMPR, a high-quality, large-scale multimodal reasoning preference dataset. and (2) on the model side, we explore integrating PO with MLLMs, developing a simple yet effective method, termed Mixed Preference Optimization (MPO), which boosts multimodal CoT performance. Our approach demonstrates improved performance across multiple benchmarks, particularly in multimodal reasoning tasks. Notably, our model, InternVL2-8B-MPO, achieves an accuracy of 67.0 on MathVista, outperforming InternVL2-8B by 8.7 points and achieving performance comparable to the 10x larger InternVL2-76B. We hope this study could inspire further advancements in MLLMs. Code, data, and model shall be publicly released.

VLM에 대한 Preference Tuning인데 Preference 데이터셋을 정답이 있는 사례에 대해서는 정답 여부로, 정답이 딱히 없는 경우에는 이미지를 주고 생성한 결과를 Positive, 그리고 이미지로 생성한 결과의 일부를 가져와 이미지 없이 나머지를 생성한 결과를 Negative로 세팅하는 식으로 구축했군요.

<english>
Preference tuning for VLM, and built preference dataset by utilizing correctness for samples with easily accessible solutions, and for instructions without definite solutions, regard generations given image as a positive, and partial text with image but completed without the image as a negative.
</english>

#preference #vision-language 