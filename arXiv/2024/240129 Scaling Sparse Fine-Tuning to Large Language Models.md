https://arxiv.org/abs/2401.16405

*Scaling Sparse Fine-Tuning to Large Language Models* (Alan Ansell, Ivan Vulić, Hannah Sterz, Anna Korhonen, Edoardo M. Ponti)

> Large Language Models (LLMs) are difficult to fully fine-tune (e.g., with instructions or human feedback) due to their sheer number of parameters. A family of parameter-efficient sparse fine-tuning (SFT) methods have proven promising in terms of performance but their memory requirements increase proportionally to the size of the LLMs. In this work, we scale sparse fine-tuning to state-of-the-art LLMs like LLaMA 2 7B and 13B. At any given time, for a desired density level, we maintain an array of parameter indices and the deltas of these parameters relative to their pretrained values. We iterate among: (a) updating the active deltas, (b) pruning indices (based on the change of magnitude of their deltas) and (c) regrowth of indices. For regrowth, we explore two criteria based on either the accumulated gradients of a few candidate parameters or their approximate momenta estimated using the efficient SM3 optimizer. We experiment with instruction-tuning of LLMs on standard dataset mixtures, finding that SFT is often superior to popular parameter-efficient fine-tuning methods like LoRA (low-rank adaptation) in terms of performance and comparable in terms of run time. We additionally show that SFT is compatible with both quantization and efficient optimizers, to facilitate scaling to ever-larger model sizes. We release the code for SFT at https://github.com/AlanAnsell/peft and for the instruction-tuning experiments at https://github.com/ducdauge/sft-llm.

Sparse Weight를 사용해 Parameter Efficient Tuning을 하는 방법. 최근에도 LoRA에 Sparse Weight를 같이 사용한 방법이 나왔었죠. (https://arxiv.org/abs/2401.04679) Sparse Weight를 사용하는 방법이 LoRA 단독으로는 충분하지 않은 영역까지 커버하는데 도움이 될지 궁금하네요. 다만 Parameter Efficient Tuning의 추가적인 가치는 파인튜닝된 다수의 모델들을 배포하는 것일 텐데 그 문제는 좀 어렵게 만들 것 같긴 합니다.

#sparsity #efficient-training

Prameter Efficieht Tuning method with sprase weight. Recently a study published which emlpoyed both LoRA and sparse weights. It could be useful if it is helpful to improve cases where using LoRA alone is not enough for gain high performances. But one important value of parameter efficient tuning is in deploying various fine tune models efficiently, but I think thses sparse weight method will make it hard.

# Links

