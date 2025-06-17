https://arxiv.org/abs/2309.00754

Efficient RLHF: Reducing the Memory Usage of PPO (Michael Santacroce, Yadong Lu, Han Yu, Yuanzhi Li, Yelong Shen)

rlhf 비용 감소. lora를 썼다는 부분에서 예상할 수 있듯 actor, critic에 대해 lora adapter 교체로 대응하고 ref는 lora를 끄는 방식으로 대응, 그리고 actor에 헤드를 두 개 달아 autoregressive generation (sft)와 preference modeling (rm)에 대응하게 한 방법입니다. 결과적으로 모델 하나에 lora adapter 2개로 ppo를 할 수 있게 되죠.

다만 오픈소스 커뮤니티에서 ppo가 인기 없는 이유는 컴퓨팅 자원과 데이터의 필요도 있지만 rlhf가 딱히 필요하지 않다는 분위기도 한 몫 하는 것 같네요.

#rl #alignment 