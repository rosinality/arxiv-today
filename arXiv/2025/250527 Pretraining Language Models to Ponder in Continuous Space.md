https://arxiv.org/abs/2505.20674

*Pretraining Language Models to Ponder in Continuous Space* (Boyi Zeng, Shixiang Song, Siyuan Huang, Yixuan Wang, He Li, Ziwei He, Xinbing Wang, Zhiyu Li, Zhouhan Lin)

> Humans ponder before articulating complex sentence elements, enabling deeper cognitive processing through focused effort. In this work, we introduce this pondering process into language models by repeatedly invoking the forward process within a single token generation step. During pondering, instead of generating an actual token sampled from the prediction distribution, the model ponders by yielding a weighted sum of all token embeddings according to the predicted token distribution. The generated embedding is then fed back as input for another forward pass. We show that the model can learn to ponder in this way through self-supervised learning, without any human annotations. Our method is straightforward and can be seamlessly integrated with various existing language models. Experiments across three widely used open-source architectures-GPT-2, Pythia, and LLaMA-and extensive downstream task evaluations demonstrate the effectiveness and generality of our method. For language modeling tasks, pondering language models achieve performance comparable to vanilla models with twice the number of parameters. On 9 downstream benchmarks, our pondering-enhanced Pythia models significantly outperform the official Pythia models. Notably, pondering-enhanced Pythia-1B is comparable to TinyLlama-1.1B, which is trained on 10 times more data. The code is available at https://github.com/LUMIA-Group/PonderingLM.

임베딩 가중합으로 Latent Thought를 구성한다는 아이디어를 생각 이상으로 많이 시도하고 있었네요. 여기서는 이 가중합을 중간 입력으로 사용해서 프리트레이닝을 한다는 형태라서 Looped Transformer와 비슷하네요.

<english>
Many researchers tried the idea of constructing latent thought using weighted sum of embeddings, more than what I expected. It is similar to looped transformer as this works tried to do pretraining by using this weighted combination as an intermediate inputs.
</english>

#transformer #llm 