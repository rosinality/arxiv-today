https://arxiv.org/abs/2311.04850

Rethinking Benchmark and Contamination for Language Models with Rephrased Samples (Shuo Yang, Wei-Lin Chiang, Lianmin Zheng, Joseph E. Gonzalez, Ion Stoica)

dataset contamination에 대한 연구. 단순히 테스트셋과 동일하거나 거의 같은 텍스트가 학습 셋에 들어가 있는 경우 뿐만 아니라 rephrase된 사례들, 단어나 숫자를 바꾸거나 순서를 바꾼다거나, 다른 언어로 번역한다거나, 코드의 경우에는 컨벤션을 바꾼다거나 무의미한 코드를 주입한다거나 하는 것들이 가능하죠. 이런 rephrase된 데이터에 대해서도 학습시키면 벤치마크 성능이 향상되지만 일반적인 N-gram overlap으로는 찾을 수 없다는 주장입니다.

그래서 LLM을 기반으로 한 contamination 탐지 알고리즘을 만들어서 돌려봤는데 instruction tuning 데이터셋에서 많게는 15~20% 정도의 오염을 발견했다고 하네요.

#dataset 