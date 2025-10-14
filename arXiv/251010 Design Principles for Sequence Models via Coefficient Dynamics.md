https://arxiv.org/abs/2510.09389

*Design Principles for Sequence Models via Coefficient Dynamics* (Jerome Sieber, Antonio Orvieto, Melanie N. Zeilinger, Carmen Amo Alonso)

> Deep sequence models, ranging from Transformers and State Space Models (SSMs) to more recent approaches such as gated linear RNNs, fundamentally compute outputs as linear combinations of past value vectors. To draw insights and systematically compare such architectures, we develop a unified framework that makes this output operation explicit, by casting the linear combination coefficients as the outputs of autonomous linear dynamical systems driven by impulse inputs. This viewpoint, in spirit substantially different from approaches focusing on connecting linear RNNs with linear attention, reveals a common mathematical theme across diverse architectures and crucially captures softmax attention, on top of RNNs, SSMs, and related models. In contrast to new model proposals that are commonly evaluated on benchmarks, we derive design principles linking architectural choices to model properties. Thereby identifying tradeoffs between expressivity and efficient implementation, geometric constraints on input selectivity, and stability conditions for numerically stable training and information retention. By connecting several insights and observations from recent literature, the framework both explains empirical successes of recent designs and provides guiding principles for systematically designing new sequence model architectures.

State Space Model의 디자인 공간의 특성. 효율적으로 구현 가능하게 하기 위한 조건(Readout 함수가 선형일 것)이 표현력을 제약함. 나머지는 그것을 어떻게 완화할 것인가의 문제.

Characteristics of the design space of state-space models. The condition for efficient implementation (linear readout function) restricts expressivity - and the rest is a matter of how to relieve it.

#state-space-model 