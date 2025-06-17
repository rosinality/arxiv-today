https://arxiv.org/abs/2308.06912

CausalLM is not optimal for in-context learning (Nan Ding, Tomer Levinboim, Jialin Wu, Sebastian Goodman, Radu Soricut)

prefix lm이 in-context learning에 대해 우수하다는 이야기. prefix lm은 in-context learning 상황에서 least square solution으로 수렴하지만 causal lm은 online gradient descent의 경로를 따르기 때문에 prefix lm이 근본적으로 우수하다는 주장입니다.

그 증거로 palm 2를 flan에 대해 prefix lm 혹은 causal lm으로 학습시킨 결과를 비교하고 있네요. palm 2 report의 결과와 어떻게 조합해서 생각할 수 있을지가 좀 모호하긴 합니다.

prefix lm은 자주 나오는 떡밥인데 좋다는 결과도 있고 애매하다는 결과도 있어서 정말 애매하네요. 구글 쪽에서는 좋아하는 것 같긴 한데요.

#lm 