https://arxiv.org/abs/2408.16293

*Physics of Language Models: Part 2.2, How to Learn From Mistakes on Grade-School Math Problems* (Tian Ye, Zicheng Xu, Yuanzhi Li, Zeyuan Allen-Zhu)

> Language models have demonstrated remarkable performance in solving reasoning tasks; however, even the strongest models still occasionally make reasoning mistakes. Recently, there has been active research aimed at improving reasoning accuracy, particularly by using pretrained language models to "self-correct" their mistakes via multi-round prompting. In this paper, we follow this line of work but focus on understanding the usefulness of incorporating "error-correction" data directly into the pretraining stage. This data consists of erroneous solution steps immediately followed by their corrections. Using a synthetic math dataset, we show promising results: this type of pretrain data can help language models achieve higher reasoning accuracy directly (i.e., through simple auto-regression, without multi-round prompting) compared to pretraining on the same amount of error-free data. We also delve into many details, such as (1) how this approach differs from beam search, (2) how such data can be prepared, (3) whether masking is needed on the erroneous tokens, (4) the amount of error required, (5) whether such data can be deferred to the fine-tuning stage, and many others.

GSM 스타일의 합성 데이터로 LLM의 추론 과정을 분석했습니다. 1. 모델은 보통 실수를 했다면 그 사실을 인식할 수 있다는 것 2. 프리트레이닝에 이렇게 실수하고 재시도하는 데이터를 주입하면 성능을 높일 수 있다는 것 3. 재시도하는 데이터는 부정확하더라도 의미가 있을 수 있다는 것 정도가 요점이겠네요.

반복해서 나오는 이야기인 텍스트에는 사고 과정이 포함되어 있지 않다는 문제의 연장선에 있는 듯 합니다. 문장과 문장 사이를 연결하는 사고 과정에는 가능한 다른 문장을 생각해보았다가 별로였다면 버리는 종류의 과정 또한 포함되어 있겠죠. 그것을 채우는 것이 다음 단계의 LLM에는 중요하리라고 봅니다.

혹은 Lean 같은 Verifier를 사용하는 경우에는 직접적으로 실수를 시뮬레이션하는 것도 충분히 가능하겠네요.

#llm #reasoning #synthetic-data 