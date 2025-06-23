https://arxiv.org/abs/2506.15545

*RATTENTION: Towards the Minimal Sliding Window Size in Local-Global Attention Models* (Bailin Wang, Chang Lan, Chong Wang, Ruoming Pang)

> Local-global attention models have recently emerged as compelling alternatives to standard Transformers, promising improvements in both training and inference efficiency. However, the crucial choice of window size presents a Pareto tradeoff: larger windows maintain performance akin to full attention but offer minimal efficiency gains in short-context scenarios, while smaller windows can lead to performance degradation. Current models, such as Gemma2 and Mistral, adopt conservative window sizes (e.g., 4096 out of an 8192 pretraining length) to preserve performance. This work investigates strategies to shift this Pareto frontier, enabling local-global models to achieve efficiency gains even in short-context regimes. Our core motivation is to address the intrinsic limitation of local attention -- its complete disregard for tokens outside the defined window. We explore RATTENTION, a variant of local attention integrated with a specialized linear attention mechanism designed to capture information from these out-of-window tokens. Pretraining experiments at the 3B and 12B scales demonstrate that RATTENTION achieves a superior Pareto tradeoff between performance and efficiency. As a sweet spot, RATTENTION with a window size of just 512 consistently matches the performance of full-attention models across diverse settings. Furthermore, the recurrent nature inherent in the linear attention component of RATTENTION contributes to enhanced long-context performance, as validated on the RULER benchmark. Crucially, these improvements do not compromise training efficiency; thanks to a specialized kernel implementation and the reduced window size, RATTENTION maintains training speeds comparable to existing state-of-the-art approaches.

Local-Global Attention의 하이브리드에서 최적 Local Window의 크기는 무엇인가? 여기서는 단순히 Local Attention을 쓰지는 않고 Linear Attention도 결합했군요.

<english>
What is the opitmal size of local window in local-global attention hybrids? This works did not used local attention simply, they also combined linear attention.
</english>

#transformer #efficiency 