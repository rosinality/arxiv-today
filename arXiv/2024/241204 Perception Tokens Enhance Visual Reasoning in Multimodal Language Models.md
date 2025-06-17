https://arxiv.org/abs/2412.03548

*Perception Tokens Enhance Visual Reasoning in Multimodal Language Models* (Mahtab Bigverdi, Zelun Luo, Cheng-Yu Hsieh, Ethan Shen, Dongping Chen, Linda G. Shapiro, Ranjay Krishna)

> Multimodal language models (MLMs) still face challenges in fundamental visual perception tasks where specialized models excel. Tasks requiring reasoning about 3D structures benefit from depth estimation, and reasoning about 2D object instances benefits from object detection. Yet, MLMs can not produce intermediate depth or boxes to reason over. Finetuning MLMs on relevant data doesn't generalize well and outsourcing computation to specialized vision tools is too compute-intensive and memory-inefficient. To address this, we introduce Perception Tokens, intrinsic image representations designed to assist reasoning tasks where language is insufficient. Perception tokens act as auxiliary reasoning tokens, akin to chain-of-thought prompts in language models. For example, in a depth-related task, an MLM augmented with perception tokens can reason by generating a depth map as tokens, enabling it to solve the problem effectively. We propose AURORA, a training method that augments MLMs with perception tokens for improved reasoning over visual inputs. AURORA leverages a VQVAE to transform intermediate image representations, such as depth maps into a tokenized format and bounding box tokens, which is then used in a multi-task training framework. AURORA achieves notable improvements across counting benchmarks: +10.8% on BLINK, +11.3% on CVBench, and +8.3% on SEED-Bench, outperforming finetuning approaches in generalization across datasets. It also improves on relative depth: over +6% on BLINK. With perception tokens, AURORA expands the scope of MLMs beyond language-based reasoning, paving the way for more effective visual reasoning capabilities.

특정한 이미지 과제에 대해서는 Depth Map 같은 정보가 추가로 주어진다면 풀기 쉬워질 수 있죠. Chain of Thought처럼 이런 정보를 생성해 예측하게 만드는 방법입니다. 이미지 생성 능력을 갖춘다면 이미지를 통해 추론하는 것도 재미있는 방향이라고 생각합니다.

현재 Chain of Thought는 어떤 텍스트를 생성할 것인지 자체에 대해서는 Supervision을 주지 않는 것이 흐름인데 이미지에 대해서 만약 이런 형태로 Chain of Thought를 학습시킨다면 어떤 이미지를 생성하게 될지 궁금하네요.

<english>
For some image related tasks it would be easier to solve when additional informations like depth maps are given. This method let model to predict by generate these kind of informations like chain of thoughts. I think it would be interesting research direction to make model reason through images if model have image generation capabilities.

Currently main idea of research on chain of thought is that we don't give a supervision on the model about which text would be generated in thought tokens. If we apply these kind of approaches to image chain of thought, I wonder what kind of images model would generate.
</english>

#reasoning 