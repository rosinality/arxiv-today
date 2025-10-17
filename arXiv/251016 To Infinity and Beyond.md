https://arxiv.org/abs/2510.14826

*To Infinity and Beyond: Tool-Use Unlocks Length Generalization in State Space Models* (Eran Malach, Omid Saremi, Sinead Williamson, Arwen Bradley, Aryo Lotfi, Emmanuel Abbe, Josh Susskind, Etai Littwin)

> State Space Models (SSMs) have become the leading alternative to Transformers for sequence modeling. Their primary advantage is efficiency in long-context and long-form generation, enabled by fixed-size memory and linear scaling of computational complexity. We begin this work by showing a simple theoretical result stating that SSMs cannot accurately solve any ``truly long-form'' generation problem (in a sense we formally define), undermining their main competitive advantage. However, we show that this limitation can be mitigated by allowing SSMs interactive access to external tools. In fact, we show that given the right choice of tool access and problem-dependent training data, SSMs can learn to solve any tractable problem and generalize to arbitrary problem length/complexity (i.e., achieve length generalization). Following our theoretical finding, we demonstrate that tool-augmented SSMs achieve remarkable length generalization on a variety of arithmetic, reasoning, and coding tasks. These findings highlight SSMs as a potential efficient alternative to Transformers in interactive tool-based and agentic settings.

SSM은 상태의 크기가 제한되어 있기에 Long-form 생성이 불가능. 하지만 만약 (Differentiable Memory 같은 것 대신) 메모리 도구를 사용해 튜링 머신을 시뮬레이션한다면 길이 일반화가 가능할 수 있음.

도구 사용이 Long Context 문제를 해결하는 한 가지 방법이 아닐까 생각.

SSMs cannot do long-form generation as their state size is bounded. But if we simulate a turing machine using memory tools (instead of things like differentiable memory), then length generalization could be possible.

In general I suspect tool use is one possibility to tackle long context problems.

#state-space-model 