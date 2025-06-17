https://arxiv.org/abs/2402.00396

*Efficient Exploration for LLMs* (Vikranth Dwaracherla, Seyed Mohammad Asghari, Botao Hao, Benjamin Van Roy)

> We present evidence of substantial benefit from efficient exploration in gathering human feedback to improve large language models. In our experiments, an agent sequentially generates queries while fitting a reward model to the feedback received. Our best-performing agent generates queries using double Thompson sampling, with uncertainty represented by an epistemic neural network. Our results demonstrate that efficient exploration enables high levels of performance with far fewer queries. Further, both uncertainty estimation and the choice of exploration scheme play critical roles.

Preference 어노테이션을 할 페어를 어떻게 샘플링할 것인가? 그냥 두 개 뽑는 대신 Reward Model, 특히 Epistemic Neural Networks (https://arxiv.org/abs/2107.08924) 를 적용한 Reward Model을 사용해 Reward Score가 높거나 혹은 Uncertanity가 높은 샘플을 쓴다는 방식입니다. 이것도 일종의 Active Learning이라고 할 수 있겠죠.

여담이지만 구글이 실험에 제미니를 쓰기 시작했군요.

#reward-model #active-learning

How should we sample to do preference annotation? Instead of just sample 2 responses, this study utilizes reward model, especially that epistemic neural network is applied. So using reward model make a sample with high reward scores or more uncertain samples. This can be think as an active learning.

Besides, this paper show Google is starting to use Gemini for experiments.

# Links

