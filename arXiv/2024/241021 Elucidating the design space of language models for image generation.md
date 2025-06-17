https://arxiv.org/abs/2410.16257

*Elucidating the design space of language models for image generation* (Xuantong Liu, Shaozhe Hao, Xianbiao Qi, Tianyang Hu, Jun Wang, Rong Xiao, Yuan Yao)

> The success of autoregressive (AR) language models in text generation has inspired the computer vision community to adopt Large Language Models (LLMs) for image generation. However, considering the essential differences between text and image modalities, the design space of language models for image generation remains underexplored. We observe that image tokens exhibit greater randomness compared to text tokens, which presents challenges when training with token prediction. Nevertheless, AR models demonstrate their potential by effectively learning patterns even from a seemingly suboptimal optimization problem. Our analysis also reveals that while all models successfully grasp the importance of local information in image generation, smaller models struggle to capture the global context. In contrast, larger models showcase improved capabilities in this area, helping to explain the performance gains achieved when scaling up model size. We further elucidate the design space of language models for vision generation, including tokenizer choice, model choice, model scalability, vocabulary design, and sampling strategy through extensive comparative experiments. Our work is the first to analyze the optimization behavior of language models in vision generation, and we believe it can inspire more effective designs when applying LMs to other domains. Finally, our elucidated language model for image generation, termed as ELM, achieves state-of-the-art performance on the ImageNet 256*256 benchmark. The code is available at https://github.com/Pepperlll/LMforImageGeneration.git.

VQ vs Binary Quantization, AR vs MLM, Binary Quantization을 쪼개 Factorize된 코드를 예측하는 방법 등에 대한 비교 실험이군요. 이미지 생성 측면에서는 디자인 공간이 여전히 넓어서 그 부분에 대한 증거를 수집하는 것이 굉장히 중요한 작업이라는 생각을 합니다.

<english>
VQ vs binary quantization, AR vs MLM, and factorizing binary quantization into multiple group codes. Design space of image generation is vastly large, and I think gathering evidence of this problem itself is very important work.
</english>

#vq #autoregressive-model #image-generation 