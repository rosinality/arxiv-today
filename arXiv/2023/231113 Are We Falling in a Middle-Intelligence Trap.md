https://arxiv.org/abs/2311.07468

Are We Falling in a Middle-Intelligence Trap? An Analysis and Mitigation of the Reversal Curse (Ang Lv, Kaiyi Zhang, Shufang Xie, Quan Tu, Yuhan Chen, Ji-Rong Wen, Rui Yan)

Reversal Curse (https://arxiv.org/abs/2309.12288) 가 꽤 화제가 되는 것 같군요. (https://nonint.com/2023/10/18/is-the-reversal-curse-a-generalization-problem/) Autoregressive LM의 기본적 혹은 근본적인 한계로 생각할 수 있는 것들이 있는데 그걸 아주 간단하게 보여주는 사례인 것 같습니다. 결국 이런 질문이죠. 이런 명백한 한계가 있는데 이 모델에 대한 Scaling으로 AGI를 달성할 수 있을까?

사실 이 문제에 대해서는 Autoregressive loss와 Causal masking이 문제일 것이라고 생각할 수 있죠. 여기서는 GLM (https://arxiv.org/abs/2210.02414) 스타일로 기존의 Llama 모델을 가져와서 bidirectional attention을 사용한 infilling objective를 적용하는 방법을 고안했습니다. UL2 (https://arxiv.org/abs/2205.05131) 도 그렇고 이런 형태의 변형 중에 의미있는 것이 있을 수 있지 않을까 하는 생각이 드네요.

#autoregressive_model #lm

# Links

[[230921 The Reversal Curse.md]]
[[220510 UL2.md]]