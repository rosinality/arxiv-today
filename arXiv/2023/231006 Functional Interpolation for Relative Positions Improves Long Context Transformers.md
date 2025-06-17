https://arxiv.org/abs/2310.04418

Functional Interpolation for Relative Positions Improves Long Context Transformers (Shanda Li, Chong You, Guru Guruganesh, Joshua Ainslie, Santiago Ontanon, Manzil Zaheer, Sumit Sanghai, Yiming Yang, Sanjiv Kumar, Srinadh Bhojanapalli)

extrapolation을 목표로 한 relative positional encoding이군요. attention bias를 relative distance을 사용해 생성하는데, 생성 함수의 입력에서 relative distance를 query의 위치로 normalize 해주는 것이 포인트입니다. 즉 b(i, j) = f((i - j) / i) 형태가 되는 것이죠. 흥미롭네요.

#positional_encoding #long_context 