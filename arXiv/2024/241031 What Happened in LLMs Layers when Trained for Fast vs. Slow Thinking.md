https://arxiv.org/abs/2410.23743

*What Happened in LLMs Layers when Trained for Fast vs. Slow Thinking: A Gradient Perspective* (Ming Li, Yanhong Li, Tianyi Zhou)

> What makes a difference in the post-training of LLMs? We investigate the training patterns of different layers in large language models (LLMs), through the lens of gradient, when training with different responses and initial models. We are specifically interested in how fast vs. slow thinking affects the layer-wise gradients, given the recent popularity of training LLMs on reasoning paths such as chain-of-thoughts (CoT) and process rewards. In our study, fast thinking without CoT leads to larger gradients and larger differences of gradients across layers than slow thinking (Detailed CoT), indicating the learning stability brought by the latter. Moreover, pre-trained LLMs are less affected by the instability of fast thinking than instruction-tuned LLMs. Additionally, we study whether the gradient patterns can reflect the correctness of responses when training different LLMs using slow vs. fast thinking paths. The results show that the gradients of slow thinking can distinguish correct and irrelevant reasoning paths. As a comparison, we conduct similar gradient analyses on non-reasoning knowledge learning tasks, on which, however, trivially increasing the response length does not lead to similar behaviors of slow thinking. Our study strengthens fundamental understandings of LLM training and sheds novel insights on its efficiency and stability, which pave the way towards building a generalizable System-2 agent. Our code, data, and gradient statistics can be found in: https://github.com/MingLiiii/Layer_Gradient.

자세한 Chain of Thought가 주어진 경우, 그리고 정답이 주어진 경우가 오답이 주어진 경우보다 레이어 사이의 그래디언트 Nuclear Norm의 차이가 줄어든다는 결과. 지식과 관련된 경우에는 입력의 길이나 오답 여부에 따른 차이가 잘 나타나지 않았다고 하네요. 직관적이면서도 흥미롭군요.

<english>
Difference of nuclear norm of gradient between each layers is decreased if detailed chain-of-thought is given, and correct answers instead of incorrect one. If the problem is knowledge-related then difference due to input length or correctness was not evident. Intuitive and interesting results.
</english>

#reasoning 