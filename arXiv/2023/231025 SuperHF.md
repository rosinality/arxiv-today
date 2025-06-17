https://arxiv.org/abs/2310.16763

SuperHF: Supervised Iterative Learning from Human Feedback (Gabriel Mukobi, Peter Chatain, Su Fong, Robert Windesheim, Gitta Kutyniok, Kush Bhatia, Silas Alberti)

Policy로 샘플링하고, 샘플들을 Reward Model로 랭킹해서 K개 뽑아내고, K개 뽑아낸 샘플로 SFT 하고, 추가로 KL penalty를 붙여서 RLHF를 하는 알고리즘. 샘플링하고 Reward Model로 걸러낸 샘플에 대해 SFT를 한다는 비슷한 알고리즘들이 여럿 나오고 괜찮은 결과들을 보고하고 있는 것을 보면 충분히 가능한 방법이 아닌가 싶기도 합니다. PPO도 오랫동안 튜닝한 결과라고 하고 있는 걸 보면 유의미한 비교가 아닐까 싶고요. Negative sample의 사용은 필요하지 않은 걸까요? 이 부분도 관심이 가는 군요.

#rlhf #alignment 

[[230529 Direct Preference Optimization]]
[[230517 SLiC-HF]]
[[230913 Statistical Rejection Sampling Improves Preference Optimization]]