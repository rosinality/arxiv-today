https://arxiv.org/abs/2309.16240

Beyond Reverse KL: Generalizing Direct Preference Optimization with Diverse Divergence Constraints (Chaoqi Wang, Yibo Jiang, Chenghao Yang, Han Liu, Yuxin Chen)

RLHF 과정의 reverse KL 페널티를 다른 divergence로 바꿔 보려는 시도. reverse KL을 쓰면 diversity가 감소하지 않는가 하는 아이디어가 동기가 되죠. Direct Preference Optimization (https://arxiv.org/abs/2305.18290) 기반으로 loss에서 log 대신 다른 함수를 사용하는 방식으로 수정되는 군요. 이 loss는 다른 offline 세팅에서도 사용될 수 있으니 (https://arxiv.org/abs/2309.06657) 재미있을 것 같네요. 결국 diversity와 accuracy의 trade off 곡선 위에서 움직이는 것이긴 합니다만.

#alignment

# Links

[[230529 Direct Preference Optimization.md]]
[[230913 Statistical Rejection Sampling Improves Preference Optimization.md]]