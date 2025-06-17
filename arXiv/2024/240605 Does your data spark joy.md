https://arxiv.org/abs/2406.03476

*Does your data spark joy? Performance gains from domain upsampling at the end of training* (Cody Blakeney, Mansheej Paul, Brett W. Larsen, Sean Owen, Jonathan Frankle)

> Pretraining datasets for large language models (LLMs) have grown to trillions of tokens composed of large amounts of CommonCrawl (CC) web scrape along with smaller, domain-specific datasets. It is expensive to understand the impact of these domain-specific datasets on model capabilities as training at large FLOP scales is required to reveal significant changes to difficult and emergent benchmarks. Given the increasing cost of experimenting with pretraining data, how does one determine the optimal balance between the diversity in general web scrapes and the information density of domain specific data? In this work, we show how to leverage the smaller domain specific datasets by upsampling them relative to CC at the end of training to drive performance improvements on difficult benchmarks. This simple technique allows us to improve up to 6.90 pp on MMLU, 8.26 pp on GSM8K, and 6.17 pp on HumanEval relative to the base data mix for a 7B model trained for 1 trillion (T) tokens, thus rivaling Llama-2 (7B)$\unicode{x2014}$a model trained for twice as long. We experiment with ablating the duration of domain upsampling from 5% to 30% of training and find that 10% to 20% percent is optimal for navigating the tradeoff between general language modeling capabilities and targeted benchmarks. We also use domain upsampling to characterize at scale the utility of individual datasets for improving various benchmarks by removing them during this final phase of training. This tool opens up the ability to experiment with the impact of different pretraining datasets at scale, but at an order of magnitude lower cost compared to full pretraining runs.

학습 스케줄의 페이즈를 나눠 데이터셋 비율을 바꾸는 트릭에 대한 연구가 나왔군요. 학습 후반에 고가치 데이터소스의 비율을 높였을 때 성능이 어떻게 변화하는가에 대한 결과입니다.

논문에서 제안하는 것은 이 트릭을 통해 성능을 높일 수 있다 뿐만 아니라 데이터셋의 비율 설정, 데이터셋의 가치나 효과 등을 좀 더 효과적으로 탐색할 수 있는 방법이 아니겠는가 하는 것이네요. Constant Learning Rate + Cooldown (https://arxiv.org/abs/2405.18392) 스케줄과도 잘 맞을 듯 합니다.

#llm

# Links

[[240528 Scaling Laws and Compute-Optimal Training Beyond Fixed Training Durations.md]]