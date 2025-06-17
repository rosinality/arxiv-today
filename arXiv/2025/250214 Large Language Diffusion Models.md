https://arxiv.org/abs/2502.09992

*Large Language Diffusion Models* (Shen Nie, Fengqi Zhu, Zebin You, Xiaolu Zhang, Jingyang Ou, Jun Hu, Jun Zhou, Yankai Lin, Ji-Rong Wen, Chongxuan Li)

> Autoregressive models (ARMs) are widely regarded as the cornerstone of large language models (LLMs). We challenge this notion by introducing LLaDA, a diffusion model trained from scratch under the pre-training and supervised fine-tuning (SFT) paradigm. LLaDA models distributions through a forward data masking process and a reverse process, parameterized by a vanilla Transformer to predict masked tokens. By optimizing a likelihood bound, it provides a principled generative approach for probabilistic inference. Across extensive benchmarks, LLaDA demonstrates strong scalability, outperforming our self-constructed ARM baselines. Remarkably, LLaDA 8B is competitive with strong LLMs like LLaMA3 8B in in-context learning and, after SFT, exhibits impressive instruction-following abilities in case studies such as multi-turn dialogue. Moreover, LLaDA addresses the reversal curse, surpassing GPT-4o in a reversal poem completion task. Our findings establish diffusion models as a viable and promising alternative to ARMs, challenging the assumption that key LLM capabilities discussed above are inherently tied to ARMs.

8B/2.3T 규모의 Masked Diffusion 모델이 나왔군요. Discrete Diffusion 쪽 연구도 최근 좀 나오고 있네요. (https://arxiv.org/abs/2502.09622) 다만 Masked Diffusion의 특성에 대해서는 분석이 필요할 듯 합니다. (토큰 다양성 등, https://arxiv.org/abs/2409.02908)

<english>
8B/2.3T scale masked diffusion language model is released. Recently some researches on discrete diffusions are appearing (https://arxiv.org/abs/2502.09622). But we may need more researches on characteristics of masked diffusion models (like token diversity, https://arxiv.org/abs/2409.02908)
</english>

#diffusion 