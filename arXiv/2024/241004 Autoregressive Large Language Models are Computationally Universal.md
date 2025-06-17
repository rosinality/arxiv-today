https://arxiv.org/abs/2410.03170

*Autoregressive Large Language Models are Computationally Universal* (Dale Schuurmans, Hanjun Dai, Francesco Zanini)

> We show that autoregressive decoding of a transformer-based language model can realize universal computation, without external intervention or modification of the model's weights. Establishing this result requires understanding how a language model can process arbitrarily long inputs using a bounded context. For this purpose, we consider a generalization of autoregressive decoding where, given a long input, emitted tokens are appended to the end of the sequence as the context window advances. We first show that the resulting system corresponds to a classical model of computation, a Lag system, that has long been known to be computationally universal. By leveraging a new proof, we show that a universal Turing machine can be simulated by a Lag system with 2027 production rules. We then investigate whether an existing large language model can simulate the behaviour of such a universal Lag system. We give an affirmative answer by showing that a single system-prompt can be developed for gemini-1.5-pro-001 that drives the model, under deterministic (greedy) decoding, to correctly apply each of the 2027 production rules. We conclude that, by the Church-Turing thesis, prompted gemini-1.5-pro-001 with extended autoregressive (greedy) decoding is a general purpose computer.

Extended Autoregressive Decoding이라는 N개 토큰의 Context Window에 대해 토큰을 생성한 다음 시퀀스 뒤에 붙이는 디코딩 알고리즘을 생각합니다. 그러면 이에 대응하는 Lag 시스템이라는, Prefix를 특정 심볼로 전환하는 알고리즘이 존재합니다. 그리고 Lag 시스템은 Universal Turing Machine을 시뮬레이션할 수 있습니다.

결과적으로 Autoregressive Decoding으로 Universal Turing Machine을 시뮬레이션하는 Lag 시스템을 시뮬레이션하는 것으로 LLM이 Universal Turing Machine이라는 것을 증명할 수 있습니다. Gemini로 해봤더니 됐다고 하네요.

좀 더 나아가서 사실 LM은 처음 시점부터 Univeral Turing Machine이고 Next Token Prediction을 통한 학습은 사람이 이해할 수 있는 인터페이스를 달아주는 과정인 것이 아닐까 하는 추측을 하는군요. 재미있습니다.

<english>
First think extended autoregressive decoding algorithm, which is for N context windows generating tokens and appending it to the tail of the sequence. Then there exists corresponding Lag system, which is converting prefix to specific symbols. And the Lag system can simulate universal turing machine.

So we can prove that Lag system which simulates universal turing machine can be simulated with autoregressive decoding. The authors tried to do it with Gemini and they found it is possible.

Furthermore, authors make a guess that maybe LM is universal turing machine at initialization time, and next token prediction just adds interface for it to human can be able to comprehend. Interesting.
</english>

#autoregressive-model #computation 