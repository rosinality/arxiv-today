https://arxiv.org/abs/2309.03450

XGen-7B Technical Report (Erik Nijkamp, Tian Xie, Hiroaki Hayashi, Bo Pang, Congying Xia, Chen Xing, Jesse Vig, Semih Yavuz, Philippe Laban, Ben Krause, Senthil Purushwalkam, Tong Niu, Wojciech Kryściński, Lidiya Murakhovs'ka, Prafulla Kumar Choubey, Alex Fabbri, Ye Liu, Rui Meng, Lifu Tu, Meghana Bhat, Chien-Sheng Wu, Silvio Savarese, Yingbo Zhou, Shafiq Joty, Caiming Xiong)

salesforce의 llm 학습 시도. 자연어 95%로 1차 학습한 다음 자연어 47.5%, 코드 52.5%로 2차 학습, 그리고 자연어 1차 학습 동안에도 3 단계로 나눠 sequence length를 증가시키면서 학습했군요. 그 외에는 llama를 많이 따라갔습니다. 학습 불안정성에 대한 이야기를 많이 하는데 parallel layer보다 sequential layer가, layer norm보다 rms norm이, gelu보다 swiglu가 더 안정적이라고 언급하는군요. 뭔가 salesforce가 코드를 주로 해보다가 자연어 모델 학습 실험을 해봤다는 느낌이 있네요.

#llm 