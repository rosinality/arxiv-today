https://arxiv.org/abs/2310.17623

Proving Test Set Contamination in Black Box Language Models (Yonatan Oren, Nicole Meister, Niladri Chatterji, Faisal Ladhak, Tatsunori B. Hashimoto)

테스트 데이터셋 오염에 대한 테스트 방법 개발. 테스트 데이터를 봤다면 테스트 데이터 내 샘플 순서대로 배치된 샘플에 대한 likelihood가 순서가 뒤바뀐 샘플의 likelihood 보다 높을 것이라는 가정 하에서 테스트했군요.

Llama-2와 Mistral에서 MMLU에 대한 오염이 의심되는 것을 발견했고, Llama-2에서 데이터셋 오염에 대해 분석한 결과를 생각해보면 타당한 결과처럼 보이네요. 흥미로운 것 중 하나는 Mistral에서 AI2-ARC에 대한 테스트셋 오염이 발견됐다는 것입니다. 원인이 무엇일지 궁금하네요.

방법에서 드러나는 한계인데 이건 테스트 데이터셋이 거의 순서대로 학습에 들어갔다는 가정을 깔고 있습니다. 그렇지만 좀 더 간접적으로 혹은 부분적으로 데이터셋 오염이 일어날 수 있는 방법은 많으니 그 부분까지는 아직 알기 어렵네요.

#dataset 