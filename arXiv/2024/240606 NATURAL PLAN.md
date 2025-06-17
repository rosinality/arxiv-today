https://arxiv.org/abs/2406.04520

*NATURAL PLAN: Benchmarking LLMs on Natural Language Planning* (Huaixiu Steven Zheng, Swaroop Mishra, Hugh Zhang, Xinyun Chen, Minmin Chen, Azade Nova, Le Hou, Heng-Tze Cheng, Quoc V. Le, Ed H. Chi, Denny Zhou)

> We introduce NATURAL PLAN, a realistic planning benchmark in natural language containing 3 key tasks: Trip Planning, Meeting Planning, and Calendar Scheduling. We focus our evaluation on the planning capabilities of LLMs with full information on the task, by providing outputs from tools such as Google Flights, Google Maps, and Google Calendar as contexts to the models. This eliminates the need for a tool-use environment for evaluating LLMs on Planning. We observe that NATURAL PLAN is a challenging benchmark for state of the art models. For example, in Trip Planning, GPT-4 and Gemini 1.5 Pro could only achieve 31.1% and 34.8% solve rate respectively. We find that model performance drops drastically as the complexity of the problem increases: all models perform below 5% when there are 10 cities, highlighting a significant gap in planning in natural language for SoTA LLMs. We also conduct extensive ablation studies on NATURAL PLAN to further shed light on the (in)effectiveness of approaches such as self-correction, few-shot generalization, and in-context planning with long-contexts on improving LLM planning.

LLM의 계획 능력 평가. 보통 Planning이라고 하면 수학 문제의 해법을 설계하기 같은 것이 가장 먼저 떠오르는 느낌이 있습니다만 여기서 제안하는 카테고리들은 주어진 제약 조건 하에서 여행 계획 만들기 같은 좀 더 캐주얼(?)한 문제들입니다.

개인적으로는 GPT-4o가 Trip Planning에서 보여주는 패턴이 좀 특이하게 느껴지네요. 이런 결과들이 나올 때마다 GPT-4o이 어떤 모델 압축 방법을 채택했기에 이런 결과로 이어지는 것일지 궁금해집니다.

#benchmark 