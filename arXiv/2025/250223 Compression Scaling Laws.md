https://arxiv.org/abs/2502.16440

*Compression Scaling Laws:Unifying Sparsity and Quantization* (Elias Frantar, Utku Evci, Wonpyo Park, Neil Houlsby, Dan Alistarh)

> We investigate how different compression techniques -- such as weight and activation quantization, and weight sparsity -- affect the scaling behavior of large language models (LLMs) during pretraining. Building on previous work showing that weight sparsity acts as a constant multiplier on model size in scaling laws, we demonstrate that this "effective parameter" scaling pattern extends to quantization as well. Specifically, we establish that weight-only quantization achieves strong parameter efficiency multipliers, while full quantization of both weights and activations shows diminishing returns at lower bitwidths. Our results suggest that different compression techniques can be unified under a common scaling law framework, enabling principled comparison and combination of these methods.

Quantization과 Sparsity에 대한 Scaling Law. 여기서는 4 bit 정도를 Pareto Frontier로 분석하고 있군요. 그런데 Quantization에 대해서는 학습량도 고려해야 한다는 이야기가 있었죠. (https://arxiv.org/abs/2411.17691)

<english>
Scaling law for quantization and sparsity. They reports around 4 bit as pareto frontier. But recently there was research saying we should consider amount of training for quantization. (https://arxiv.org/abs/2411.17691)
</english>

#scaling-law #quantization #sparsity 