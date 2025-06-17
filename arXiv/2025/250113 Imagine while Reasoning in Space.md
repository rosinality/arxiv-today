https://arxiv.org/abs/2501.07542

*Imagine while Reasoning in Space: Multimodal Visualization-of-Thought* (Chengzu Li, Wenshan Wu, Huanyu Zhang, Yan Xia, Shaoguang Mao, Li Dong, Ivan Vulić, Furu Wei)

> Chain-of-Thought (CoT) prompting has proven highly effective for enhancing complex reasoning in Large Language Models (LLMs) and Multimodal Large Language Models (MLLMs). Yet, it struggles in complex spatial reasoning tasks. Nonetheless, human cognition extends beyond language alone, enabling the remarkable capability to think in both words and images. Inspired by this mechanism, we propose a new reasoning paradigm, Multimodal Visualization-of-Thought (MVoT). It enables visual thinking in MLLMs by generating image visualizations of their reasoning traces. To ensure high-quality visualization, we introduce token discrepancy loss into autoregressive MLLMs. This innovation significantly improves both visual coherence and fidelity. We validate this approach through several dynamic spatial reasoning tasks. Experimental results reveal that MVoT demonstrates competitive performance across tasks. Moreover, it exhibits robust and reliable improvements in the most challenging scenarios where CoT fails. Ultimately, MVoT establishes new possibilities for complex reasoning tasks where visual thinking can effectively complement verbal reasoning.

이미지로 CoT를 하게 했을 때 공간적 추론에 도움이 된다는 연구. 지금은 각 과제에 대한 이미지 타겟을 직접 주는 형태이지만 만약 RL을 통해 추론을 위한 이미지를 생성할 수 있게 된다면 좀 더 재미있어질 것 같네요.

<english>
A study that it is helpful to spatial reasoning if you let model to do CoT on images. Currently model is directly trained to generated target images specific for each tasks but if we can let model to generate images for reasoning using RL then it would became more interesting.
</english>

#reasoning #multimodal 