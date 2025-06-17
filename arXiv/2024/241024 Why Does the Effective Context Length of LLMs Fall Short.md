https://arxiv.org/abs/2410.18745

*Why Does the Effective Context Length of LLMs Fall Short?* (Chenxin An, Jun Zhang, Ming Zhong, Lei Li, Shansan Gong, Yao Luo, Jingjing Xu, Lingpeng Kong)

> Advancements in distributed training and efficient attention mechanisms have significantly expanded the context window sizes of large language models (LLMs). However, recent work reveals that the effective context lengths of open-source LLMs often fall short, typically not exceeding half of their training lengths. In this work, we attribute this limitation to the left-skewed frequency distribution of relative positions formed in LLMs pretraining and post-training stages, which impedes their ability to effectively gather distant information. To address this challenge, we introduce ShifTed Rotray position embeddING (STRING). STRING shifts well-trained positions to overwrite the original ineffective positions during inference, enhancing performance within their existing training lengths. Experimental results show that without additional training, STRING dramatically improves the performance of the latest large-scale models, such as Llama3.1 70B and Qwen2 72B, by over 10 points on popular long-context benchmarks RULER and InfiniteBench, establishing new state-of-the-art results for open-source LLMs. Compared to commercial models, Llama 3.1 70B with \method even achieves better performance than GPT-4-128K and clearly surpasses Claude 2 and Kimi-chat.

Relative Distance를 생각했을 때 가까운 거리에 비해 멀리 떨어진 거리는 빈도가 작기 때문에 학습이 어렵다는 추정. Sliding Window Attention으로 가까운 거리를 모델링하고 멀리 떨어진 거리의 토큰들에 대해서는 위치를 재지정하는 것으로 대응. ReRoPE가 생각나네요. (https://github.com/bojone/rerope) 학습 시점에서부터 쓸 수 있는 무언가 좋은 Position Encoding 세팅이 있지 않을까 하는 생각이 듭니다.

<english>
Guess that relative to near distances, frequency of far distances are relative small, so it is hard to learn long range relationships. They used sliding window attention to model near distances and for far away tokens they reassigned position index. It reminds me ReRoPE (https://github.com/bojone/rerope). I think it maybe possible to design configuration of position encoding can be used at the pretraining time.
</english>

#long-context 