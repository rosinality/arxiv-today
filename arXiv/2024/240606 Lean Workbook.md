https://arxiv.org/abs/2406.03847

*Lean Workbook: A large-scale Lean problem set formalized from natural language math problems* (Huaiyuan Ying, Zijian Wu, Yihan Geng, Jiayu Wang, Dahua Lin, Kai Chen)

> Large language models have demonstrated impressive capabilities across various natural language processing tasks, especially in solving mathematical problems. However, large language models are not good at math theorem proving using formal languages like Lean. A significant challenge in this area is the scarcity of training data available in these formal languages. To address this issue, we propose a novel pipeline that iteratively generates and filters synthetic data to translate natural language mathematical problems into Lean 4 statements, and vice versa. Our results indicate that the synthetic data pipeline can provide useful training data and improve the performance of LLMs in translating and understanding complex mathematical problems and proofs. Our final dataset contains about 57K formal-informal question pairs along with searched proof from the math contest forum and 21 new IMO questions. We open-source our code at https://github.com/InternLM/InternLM-Math and our data at https://huggingface.co/datasets/InternLM/Lean-Workbook.

Lean을 사용한 Autoformalization 문제에 뛰어든 사람들이 꽤 많네요. 수학에 익숙하고 Lean 같은 언어도 알아야 하니 수작업으로 하자면 난이도가 끔찍할 것 같긴 합니다.

여하간 Proof Assistant를 사용하는 방향이 수학에 대해 중요한 진전을 만들 수 있으리라고 기대하는 사람들이 많다는 것이겠죠. 수학에 대해서 능력이 향상된다면 다른 영역에도 도움이 될까 하는 것도 중요한 문제일 듯 합니다. 코드가 추론 능력 향상에 도움이 된다는 아이디어를 보면 그런 일반화도 가능할 것 같긴 합니다.

#math 