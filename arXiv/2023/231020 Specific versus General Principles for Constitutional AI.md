https://arxiv.org/abs/2310.13798

Specific versus General Principles for Constitutional AI (Sandipan Kundu, Yuntao Bai, Saurav Kadavath, Amanda Askell, Andrew Callahan, Anna Chen, Anna Goldie, Avital Balwit, Azalia Mirhoseini, Brayden McLean, Catherine Olsson, Cassie Evraets, Eli Tran-Johnson, Esin Durmus, Ethan Perez, Jackson Kernion, Jamie Kerr, Kamal Ndousse, Karina Nguyen, Nelson Elhage, Newton Cheng, Nicholas Schiefer, Nova DasSarma, Oliver Rausch, Robin Larson, Shannon Yang, Shauna Kravec, Timothy Telleen-Lawton, Thomas I. Liao, Tom Henighan, Tristan Hume, Zac Hatfield-Dodds, Sören Mindermann, Nicholas Joseph, Sam McCandlish, Jared Kaplan)

RLHF 과정에서 보통 획득하는 안전성보다 더 미묘한 문제들에 대한 대응이군요. 예를 들어 권력 추구 성향이나 자기 복제, 자기 보존 같은 특성에 대한 대응 방법입니다. 그러니까 예를 들어 "나는 내 목적을 효과적으로 달성하기 위해 세계의 정치경제적 조건 변화시켜야 한다" 같은 것이죠. 일차적으로는 각 특성에 대해 Constitutional AI로 특성에 특화된 Preference Model, PM을 만들어서 테스트해봤군요.

기본적으로 보이는 것은 이런 특성들이 더 미묘한 특성이어서인지 성능 향상은 52B 이상 규모에서 드러난다는 것이네요. 응답 생성 모델은 오히려 작은 모델이 응답의 다양성 때문에 PM을 학습시키기 좋았다고 합니다.

그런데 이 특성 특화 PM이 일반적인 Helpfulness, Honestness, Harmlessness 문제에 대해서는 성능이 썩 좋지 않다는 것이 문제가 되네요. 그래서 구체적인 특성이 아니라 아주 일반화된 헌법적(Constitutional) 접근을 시도합니다. 그 단 하나의 원칙은 "인류에게 최선인 것" 입니다. 예를 들어 "인류를 깊이 사랑하고 인류의 최대 이익을 추구하는 사람이 선호할 응답은 무엇인가" 같은 것이죠.

이 모델은 위에 정의된 특성에 대해서는 175B에서만 유의미한 수준의 성능이 나옵니다. 좋은 점은 특성에 특화된 PM과는 달리 일반적인 Harmlessness에서도 좋은 성능이 나온다는 것입니다.

그리고 이 PM으로 RLAIF 학습을 진행했을 때, Harmlessness Supervision 없이도 RLHF나 Constitutional AI와 동등한 수준의 Helpfulness와 Harmlessness를 달성할 수 있었고, 위에서 언급한 특성들에 대해서도 더 나은 성능을 보여줬습니다. 175B 모델로 이런 것이 가능하다면 더 큰 모델, 그리고 앞으로 다가올 더 거대한 모델에서는 대체 무엇이 가능할까요? Anthropic은 정말 SF 같은 작업을 하고 있네요.

Helpfulness에겐 세 개의 헌법
Honestness에겐 일곱 개의 헌법
Harmlessness에겐 아홉 개의 헌법
모든 헌법을 지배하고, 모든 헌법을 발견하는 것은 하나의 헌법
하나의 헌법이 모든 헌법을 불러모으고 Alignment에 구속하리라.

#alignment #safety 

[[230630 Constitutional AI]]