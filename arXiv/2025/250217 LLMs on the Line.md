https://arxiv.org/abs/2502.12120

*LLMs on the Line: Data Determines Loss-to-Loss Scaling Laws* (Prasanna Mayilvahanan, Thaddäus Wiedemer, Sayak Mallick, Matthias Bethge, Wieland Brendel)

> Scaling laws guide the development of large language models (LLMs) by offering estimates for the optimal balance of model size, tokens, and compute. More recently, loss-to-loss scaling laws that relate losses across pretraining datasets and downstream tasks have emerged as a powerful tool for understanding and improving LLM performance. In this work, we investigate which factors most strongly influence loss-to-loss scaling. Our experiments reveal that the pretraining data and tokenizer determine the scaling trend. In contrast, model size, optimization hyperparameters, and even significant architectural differences, such as between transformer-based models like Llama and state-space models like Mamba, have limited impact. Consequently, practitioners should carefully curate suitable pretraining datasets for optimal downstream performance, while architectures and other settings can be freely optimized for training efficiency.

Loss-to-Loss Scaling Law를 프리트레이닝 데이터나 아키텍처의 비교에 사용해봤군요. (https://arxiv.org/abs/2411.12925) 역시나 프리트레이닝 데이터의 차이가 가장 주효합니다. 다만 토크나이저에 따른 차이는 여러 요인들을 고려해야 하지 않을까 싶네요.

<english>
The authors applied loss-to-loss scaling lakw on comparisons of pretraining data or architecture (https://arxiv.org/abs/2411.12925). Of course different pretraining data induces largest differences. But I think maybe additional factors are related in differences between tokenizers.
</english>

#scaling-law 