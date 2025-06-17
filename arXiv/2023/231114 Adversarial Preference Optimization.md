https://arxiv.org/abs/2311.08045

Adversarial Preference Optimization (Pengyu Cheng, Yifan Yang, Jian Li, Yong Dai, Nan Du)

RLHF 과정에서 policy의 생성 분포가 RM을 학습한 분포와 달라지면서 발생하는 차이가 문제가 되죠. 이전에는 policy로 다시 생성해서 데이터를 재구축 하는 방식을 많이 썼는데, 이런 반복적인 방식을 줄일 수 있는 방법이 있지 않을까 하는 아이디어입니다. golden response가 있다고 했을 때 golden response와 policy의 샘플을 사용해서 RM을 업데이트하고, 업데이트한 RM으로 RL을 하는 방법입니다. 전반적으로 golden response와 생성 샘플을 구분하게 한다는 점에서 adversarial traning과 비슷하다는 이야기를 하고 있네요.

문제는 golden response가 있어야 한다는 것이겠죠. 여기서는 GPT-4 응답을 썼는데 실전에서는 golden response를 만드는 것이 RM 데이터를 새로 만드는 것보다 비쌀 듯 싶습니다.

#rlhf 