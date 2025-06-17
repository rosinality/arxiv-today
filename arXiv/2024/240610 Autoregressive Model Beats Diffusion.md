https://arxiv.org/abs/2406.06525

*Autoregressive Model Beats Diffusion: Llama for Scalable Image Generation* (Peize Sun, Yi Jiang, Shoufa Chen, Shilong Zhang, Bingyue Peng, Ping Luo, Zehuan Yuan)

> We introduce LlamaGen, a new family of image generation models that apply original ``next-token prediction'' paradigm of large language models to visual generation domain. It is an affirmative answer to whether vanilla autoregressive models, e.g., Llama, without inductive biases on visual signals can achieve state-of-the-art image generation performance if scaling properly. We reexamine design spaces of image tokenizers, scalability properties of image generation models, and their training data quality. The outcome of this exploration consists of: (1) An image tokenizer with downsample ratio of 16, reconstruction quality of 0.94 rFID and codebook usage of 97% on ImageNet benchmark. (2) A series of class-conditional image generation models ranging from 111M to 3.1B parameters, achieving 2.18 FID on ImageNet 256x256 benchmarks, outperforming the popular diffusion models such as LDM, DiT. (3) A text-conditional image generation model with 775M parameters, from two-stage training on LAION-COCO and high aesthetics quality images, demonstrating competitive performance of visual quality and text alignment. (4) We verify the effectiveness of LLM serving frameworks in optimizing the inference speed of image generation models and achieve 326% - 414% speedup. We release all models and codes to facilitate open-source community of visual generation and multimodal foundation models.

Autoregressive 이미지 생성에 대한 결과가 본격적으로 나오기 시작하는군요. 더 나은 토크나이저 + 데이터의 조합으로 성능을 끌어올렸습니다.

이미지 생성 자체에서는 재미있는 결과들이 많이 나오는 듯한데 다음 단계로 흥미로운 문제는 이미지 인식과 이미지 생성을 어떻게 통합할 것인가일 것 같네요. Reconstruction이 충분히 잘 된다면 토크나이저 기반 방법으로도 가능할 듯 한데 이 문제에 대한 실험 결과들이 더 나오면 흥미로울 듯 합니다. OCR 같은 과제로 테스트해보면 되지 않을까 싶네요.

#autoregressive-model #vq #image-generation 