https://arxiv.org/abs/2309.13308

Calibrating LLM-Based Evaluator (Yuxuan Liu, Tianchi Yang, Shaohan Huang, Zihan Zhang, Haizhen Huang, Furu Wei, Weiwei Deng, Feng Sun, Qi Zhang)

LLM을 사용한 평가를 사람의 평가와 어떻게 캘리브레이션할 것인가. 일단 사람의 평가 결과를 모읍니다. 평가 결과를 몇 개 샘플링해서 LLM에게 입력으로 주고 평가 기준을 생성하게 합니다. 그리고 이렇게 생성된 평가 기준 중 괜찮은 것들을 골라, 평과 결과 셋에서의 성능을 보고, 틀리는 케이스를 가져와서 다시 LLM에 입력으로 주고 평가 기준을 개선하게 합니다.

캘리브레이션이라는 목적을 걸긴 했지만 프롬프트 튜닝 기법이라는 측면에서 봐야하지 않을까 싶네요.

#evaluation #prompt 