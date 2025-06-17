https://ai.meta.com/blog/code-llama-large-language-model-coding/

소문이 돌던 Llama의 코드 버전 모델이 나왔다. 흥미로운 포인트들.

1. 기본적으로 Llama 2 모델을 가져다 코드 데이터에 대해 추가 학습한 모델이다. learning rate를 낮춰서 시작한다거나 하는 것 없이 원 learning rate를 사용해 warm restart를 했다.
2. fill in the middle을 사용해 infilling 기능이 추가됐다.
3. rope의 frequency를 수정하는 방법으로 4K에서 16K로 context length를 증가시켰다. perplexity를 관측할 수 있으면 좋을 것 같기도 한데 여튼 결과는 굉장히 성공적인 편인 것으로 보인다.
4. llama 2 데이터셋으로 instruction tuning 수행.
5. self instruct 사용. 일단 llama 2로 프롬프트를 생성한 다음, 프롬프트에 대한 코드와 유닛 테스트를 작성하고 유닛 테스트 실행 결과를 사용해 성공한 케이스의 데이터를 사용하는 것. 코드 문제에 대해 유닛 테스트를 사용하려는 흐름의 연장선상에 있다고 볼 수 있겠다.
6. code llama instruct 버전은 llama 2 chat 버전과 helpfulness는 비슷하게 유지하면서 코딩 능력이 향상된 것으로 보인다. 코드 위주의 학습 과정이 자연어에 대해서 성능에 큰 영향이 없었다는 의미일까? 그러나 gsm8k나 truthfulqa 등 영향이 보이는 사례도 있다.
7. self instruct 데이터를 사용하긴 했지만 instruct tuning 데이터에서 코딩 데이터의 부족이 한계가 된 듯 하다. unnatural instruction (https://arxiv.org/abs/2212.09689) 스타일로 데이터를 추가했을 때 HumanEval과 MBPP의 성능 향상이 상당히 크다. 다만 이 모델은 instruction tuning된 모델에서 뽑아낸 데이터로 학습한 모델이라서인지 공개는 하지 않았다.

그나저나 Llama는 데이터를 집어넣고 더 집어넣어도 loss 그래프가 꺾일 기미가 보이지 않는다. 학습을 더 오래 가져갔을 때 어디까지 도달할 수 있을지도 흥미로운 부분일 듯.

rope가 long context 문제에 대해서 가장 적절한 positional embedding일지는 잘 모르겠는데 llama가 rope를 채택했다 보니 long context tuning에 대해 가장 많은 자료가 쌓이고 있는 방법이 된 듯 하다. GPT-4나 Claude 2가 어떤 positional embedding을 쓰고 있는지는 여전히 궁금.

instruction tuning 데이터셋에 대해 proprietary라는 표현을 쓴 것이 재미있다. 물론 그게 이상한 것은 아니다. 다만 모델이 공개되더라도 그 모델을 학습한 데이터셋은 여전히 공개되지 않는다는 사실이 데이터의 중요성과 의미를 보여주는 것이 아닐까 싶다.

Llama 2의 의미 중 하나는 ChatGPT-3.5와 비슷한 수준에 도달하기 위해 어느 정도의 자원과 노력이 필요한지를 가늠할 수 있는 증거를 제공한다는 것이 아닐까 싶다. 그리고 Code Llama도 ChatGPT의 놀라운 코딩 능력에 어떻게 가까워질 수 있는지를 보여주는 듯 싶다.