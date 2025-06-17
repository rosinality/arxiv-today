https://arxiv.org/abs/2308.07921

Solving Challenging Math Word Problems Using GPT-4 Code Interpreter with Code-based Self-Verification (Aojun Zhou, Ke Wang, Zimu Lu, Weikang Shi, Sichun Luo, Zipeng Qin, Shaoqing Lu, Anya Jia, Linqi Song, Mingjie Zhan, Hongsheng Li)

코드 사용이 llm의 문제 해결 능력에 어떤 영향을 미치는지 테스트. GPT-4 코드 인터프리터를 사용해서 프롬프트로 코드 사용 횟수를 정해준 다음에 성능이 어떻게 변화하는지를 일단 관측했습니다. 코드 사용 횟수가 늘어날수록 성능이 향상된다는 것이 나타나네요.

여기에 verification을 유도하는 프롬프트를 사용해고, k개 샘플을 뽑은 뒤 verification 결과로 voting하게 만드니 50점대 점수가 나오던 MATH에서 84.32 (!)에 도달했네요. 굉장합니다.

#llm #code #reasoning 