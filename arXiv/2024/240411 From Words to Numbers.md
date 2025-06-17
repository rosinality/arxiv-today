https://arxiv.org/abs/2404.07544

*From Words to Numbers: Your Large Language Model Is Secretly A Capable Regressor When Given In-Context Examples* (Robert Vacareanu, Vlad-Andrei Negru, Vasile Suciu, Mihai Surdeanu)

> We analyze how well pre-trained large language models (e.g., Llama2, GPT-4, Claude 3, etc) can do linear and non-linear regression when given in-context examples, without any additional training or gradient updates. Our findings reveal that several large language models (e.g., GPT-4, Claude 3) are able to perform regression tasks with a performance rivaling (or even outperforming) that of traditional supervised methods such as Random Forest, Bagging, or Gradient Boosting. For example, on the challenging Friedman #2 regression dataset, Claude 3 outperforms many supervised methods such as AdaBoost, SVM, Random Forest, KNN, or Gradient Boosting. We then investigate how well the performance of large language models scales with the number of in-context exemplars. We borrow from the notion of regret from online learning and empirically show that LLMs are capable of obtaining a sub-linear regret.

In-context Learning으로 선형 회귀 뿐만 아니라 비선형 회귀도 풀 수 있다는 결과. LLM으로 이런 회귀 문제를 풀어야 할 일은 없겠지만 In-context Learning에서 Gradient Descent 같은 알고리즘이 구현된다는 아이디어의 측면에서 생각해볼 수 있겠네요. 물론 회귀 문제를 풀 수 있다는 것을 회귀 문제를 풀 수 있는 알고리즘이 들어 있다는 결과로 바로 연결할 수는 없겠지만요.

#in-context-learning 