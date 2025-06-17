https://arxiv.org/abs/2308.07124

OctoPack: Instruction Tuning Code Large Language Models (Niklas Muennighoff, Qian Liu, Armel Zebaze, Qinkai Zheng, Binyuan Hui, Terry Yue Zhuo, Swayam Singh, Xiangru Tang, Leandro von Werra, Shayne Longpre)

코드 커밋 메시지와 diff를 instruction 데이터로 사용하는 방법이네요. 흥미로운 방법인 것 같습니다. 위의 self alignment와 결합하면 더 나은 결과를 얻을 수 있을 것 같네요.그리고 self alignment와 이 연구는 ChatGPT의 결과를 사용한 방법과 그렇지 않은 방법을 구분하기 시작하고 있군요.

[[230509 StarCoder]] 사실 starcoder에도 코드 커밋 메시지를 pretrain에 사용했다. 차이라면 instruction tuning에 사용했다는 것과 필터링 방법, 프롬프트 형식인 듯.

fix에 대해서만 성능 향상이 두드러지는 것도 참조할 부분.

#code #instruct #alignment 