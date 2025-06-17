https://arxiv.org/abs/2311.17541

TaskWeaver: A Code-First Agent Framework (Bo Qiao, Liqun Li, Xu Zhang, Shilin He, Yu Kang, Chaoyun Zhang, Fangkai Yang, Hang Dong, Jue Zhang, Lu Wang, Minghua Ma, Pu Zhao, Si Qin, Xiaoting Qin, Chao Du, Yong Xu, Qingwei Lin, Saravan Rajmohan, Dongmei Zhang)

코드 작성을 기반으로 작동하는 자율 에이전트 설계. 사용자의 요청이 들어오면 요청을 분해하고 계획을 생성합니다. 이 계획 생성 과정에 예제들을 추가해 좀 더 커스터마이즈를 할 수 있게 고려했네요. 그리고 이 계획을 기반으로 코드를 작성하는데, 코드 작성 과정에서 플러그인을 설정할 수 있게 만들었네요. 그 다음 작성한 코드를 검증하고, 코드를 실행하는데 인터프리터로 한 번 실행하고 종료하는 것이 아니라 상태를 유지해서 코드를 계속 실행해나갈 수 있게 만들었습니다.

데이터 분석을 메인 시나리오로 설정하고 있는데 잘 작동한다면 꽤 재미있지 않을까 싶네요.

#agent 

[[230314 ViperGPT]]