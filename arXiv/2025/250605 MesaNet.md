https://arxiv.org/abs/2506.05233

*MesaNet: Sequence Modeling by Locally Optimal Test-Time Training* (Johannes von Oswald, Nino Scherrer, Seijin Kobayashi, Luca Versari, Songlin Yang, Maximilian Schlegel, Kaitlin Maile, Yanick Schimpf, Oliver Sieberling, Alexander Meulemans, Rif A. Saurous, Guillaume Lajoie, Charlotte Frenkel, Razvan Pascanu, Blaise Agüera y Arcas, João Sacramento)

> Sequence modeling is currently dominated by causal transformer architectures that use softmax self-attention. Although widely adopted, transformers require scaling memory and compute linearly during inference. A recent stream of work linearized the softmax operation, resulting in powerful recurrent neural network (RNN) models with constant memory and compute costs such as DeltaNet, Mamba or xLSTM. These models can be unified by noting that their recurrent layer dynamics can all be derived from an in-context regression objective, approximately optimized through an online learning rule. Here, we join this line of work and introduce a numerically stable, chunkwise parallelizable version of the recently proposed Mesa layer (von Oswald et al., 2024), and study it in language modeling at the billion-parameter scale. This layer again stems from an in-context loss, but which is now minimized to optimality at every time point using a fast conjugate gradient solver. Through an extensive suite of experiments, we show that optimal test-time training enables reaching lower language modeling perplexity and higher downstream benchmark performance than previous RNNs, especially on tasks requiring long context understanding. This performance gain comes at the cost of additional flops spent during inference time. Our results are therefore intriguingly related to recent trends of increasing test-time compute to improve performance -- here by spending compute to solve sequential optimization problems within the neural network itself.

Mesa Optimization을 (https://arxiv.org/abs/2309.05858) 시퀀스 모델링에 대해 평가해봤군요. 짧은 시퀀스에 대해서 장점이 있는데 컨텍스트가 길어지면 역시 트랜스포머에 밀리네요. RNN의 어쩔 수 없는 한계이긴 합니다.

<english>
Attempt to use mesa optimization for sequence modeling. It has advantage on short sequences but underperforms to transformer when context become longer. It is hard to avoid limitation of current RNNs.
</english>

#state-space-model 