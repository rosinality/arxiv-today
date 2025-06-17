https://arxiv.org/abs/2503.05592

*R1-Searcher: Incentivizing the Search Capability in LLMs via Reinforcement Learning* (Huatong Song, Jinhao Jiang, Yingqian Min, Jie Chen, Zhipeng Chen, Wayne Xin Zhao, Lei Fang, Ji-Rong Wen)

> Existing Large Reasoning Models (LRMs) have shown the potential of reinforcement learning (RL) to enhance the complex reasoning capabilities of Large Language Models~(LLMs). While they achieve remarkable performance on challenging tasks such as mathematics and coding, they often rely on their internal knowledge to solve problems, which can be inadequate for time-sensitive or knowledge-intensive questions, leading to inaccuracies and hallucinations. To address this, we propose \textbf{R1-Searcher}, a novel two-stage outcome-based RL approach designed to enhance the search capabilities of LLMs. This method allows LLMs to autonomously invoke external search systems to access additional knowledge during the reasoning process. Our framework relies exclusively on RL, without requiring process rewards or distillation for a cold start. % effectively generalizing to out-of-domain datasets and supporting both Base and Instruct models. Our experiments demonstrate that our method significantly outperforms previous strong RAG methods, even when compared to the closed-source GPT-4o-mini.

검색 도구 사용을 RL로 주입하려는 시도. 도구를 반복적으로 사용하도록 RL로 학습시키는 것은 자연스러운 발전 방향이겠죠. (Deep Research에서도 비슷한 방법을 사용했을 것 같고요.)

<english>
The author tried to inject search tool use by RL. It is natural development to train model to use tools repeatedly using RL. (Maybe Deep Research would have used similar methods.)
</english>

#reasoning #lm 