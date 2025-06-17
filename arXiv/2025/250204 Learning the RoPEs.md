https://arxiv.org/abs/2502.02562

*Learning the RoPEs: Better 2D and 3D Position Encodings with STRING* (Connor Schenck, Isaac Reid, Mithun George Jacob, Alex Bewley, Joshua Ainslie, David Rendleman, Deepali Jain, Mohit Sharma, Avinava Dubey, Ayzaan Wahid, Sumeet Singh, Rene Wagner, Tianli Ding, Chuyuan Fu, Arunkumar Byravan, Jake Varley, Alexey Gritsenko, Matthias Minderer, Dmitry Kalashnikov, Jonathan Tompson, Vikas Sindhwani, Krzysztof Choromanski)

> We introduce STRING: Separable Translationally Invariant Position Encodings. STRING extends Rotary Position Encodings, a recently proposed and widely used algorithm in large language models, via a unifying theoretical framework. Importantly, STRING still provides exact translation invariance, including token coordinates of arbitrary dimensionality, whilst maintaining a low computational footprint. These properties are especially important in robotics, where efficient 3D token representation is key. We integrate STRING into Vision Transformers with RGB(-D) inputs (color plus optional depth), showing substantial gains, e.g. in open-vocabulary object detection and for robotics controllers. We complement our experiments with a rigorous mathematical analysis, proving the universality of our methods.

RoPE의 일반화. Q와 K 각각에 대한 변환으로 분할 가능하고 이동에 불변인 PE 중에서는 가장 일반적인 형태라고 하는군요. 결과적으로는 RoPE와 닮은 형태인데 이 기저 변환을 명시적으로 학습하는 것이 도움이 되는 것 같다고 하네요.

<english>
A generalization of RoPE. The paper insist that it is most generalized form that separable into transform on Q and K, and translational invariant. It is similar to RopE matrix but the authors says explicit training of these change of basis could be helpful.
</english>

#positional-encoding 