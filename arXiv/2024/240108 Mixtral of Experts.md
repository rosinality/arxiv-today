https://arxiv.org/abs/2401.04088

*Mixtral of Experts* (Albert Q. Jiang, Alexandre Sablayrolles, Antoine Roux, Arthur Mensch, Blanche Savary, Chris Bamford, Devendra Singh Chaplot, Diego de las Casas, Emma Bou Hanna, Florian Bressand, Gianna Lengyel, Guillaume Bour, Guillaume Lample, Lélio Renard Lavaud, Lucile Saulnier, Marie-Anne Lachaux, Pierre Stock, Sandeep Subramanian, Sophia Yang, Szymon Antoniak, Teven Le Scao, Théophile Gervet, Thibaut Lavril, Thomas Wang, Timothée Lacroix, William El Sayed)

> We introduce Mixtral 8x7B, a Sparse Mixture of Experts (SMoE) language model. Mixtral has the same architecture as Mistral 7B, with the difference that each layer is composed of 8 feedforward blocks (i.e. experts). For every token, at each layer, a router network selects two experts to process the current state and combine their outputs. Even though each token only sees two experts, the selected experts can be different at each timestep. As a result, each token has access to 47B parameters, but only uses 13B active parameters during inference. Mixtral was trained with a context size of 32k tokens and it outperforms or matches Llama 2 70B and GPT-3.5 across all evaluated benchmarks. In particular, Mixtral vastly outperforms Llama 2 70B on mathematics, code generation, and multilingual benchmarks. We also provide a model fine-tuned to follow instructions, Mixtral 8x7B - Instruct, that surpasses GPT-3.5 Turbo, Claude-2.1, Gemini Pro, and Llama 2 70B - chat model on human benchmarks. Both the base and instruct models are released under the Apache 2.0 license.

Mixtral의 테크니컬 리포트가 나왔군요. Mistral의 리포트가 그렇듯 크게 새로운 사실은 별로 없습니다. MoE 라우팅이 도메인이나 토큰에 따라 어떻게 달라지는지에 대한 관찰은 흥미로운 부분이네요. 도메인에 따른 차이는 거의 없는 듯 하고 동일한 (연속된) 토큰에 대해 동일한 Expert로 넘어가는 패턴이 나타납니다.

이런 패턴이 나타난다는 것이 토큰 ID 기반 라우팅이 가능한 이유겠죠. 추가적으로 연속된 토큰에 대해 동일한 Expert로 연결된다는 것에서는 여러 토큰에 해당하는 라우팅용 토큰을 만들어 라우팅한 접근 (https://arxiv.org/abs/2311.10768) 이 떠오르네요. 생각해볼 여지가 있지 않을까 싶습니다.

#llm #moe

# Links

[[231115 Memory Augmented Language Models through Mixture of Word Experts.md]]