https://arxiv.org/abs/2308.12066

Pre-gated MoE: An Algorithm-System Co-Design for Fast and Scalable Mixture-of-Expert Inference (Ranggi Hwang, Jianyu Wei, Shijie Cao, Changho Hwang, Xiaohu Tang, Ting Cao, Mao Yang, Minsoo Rhu)

이젠 MS에서 MoE 관련된 논문이 왜 많이 나오는지 명확해졌죠. 이 논문에서는 MoE 레이어들을 CPU 메모리에 offloading 한 다음 MoE 레이어를 필요할 때 GPU로 전송하는 방법을 고안했네요. MoE 레이어를 사용하는 바로 그 시점에 GPU에 올리면 부하가 크니 MoE 레이어를 선택하는 게이트가 현 MoE 레이어를 선택하는 것이 아니라 다음 MoE 레이어를 선택하게 만들었네요. 사용할 MoE 레이어를 미리 알 수 있으니 전송도 미리 해놓을 수 있다는 식이군요.

#mixture_of_experts #efficiency 