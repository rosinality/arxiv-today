https://arxiv.org/abs/2411.19477

*A Simple and Provable Scaling Law for the Test-Time Compute of Large Language Models* (Yanxi Chen, Xuchen Pan, Yaliang Li, Bolin Ding, Jingren Zhou)

> We propose a general two-stage algorithm that enjoys a provable scaling law for the test-time compute of large language models (LLMs). Given an input problem, the proposed algorithm first generates N candidate solutions, and then chooses the best one via a multiple-round knockout tournament where each pair of candidates are compared for K times and only the winners move on to the next round. In a minimalistic implementation, both stages can be executed with a black-box LLM alone and nothing else (e.g., no external verifier or reward model), and a total of N×(K+1) highly parallelizable LLM calls are needed for solving an input problem. Assuming that a generated candidate solution is correct with probability p_gen > 0 and a comparison between a pair of correct and incorrect solutions identifies the right winner with probability p_comp > 0.5 (i.e., better than a random guess), we prove theoretically that the failure probability of the proposed algorithm decays to zero exponentially with respect to N and K: 
> 
> P(final output is incorrect) ≤ (1 − p_gen)^N + ⌈log2N⌉e^(−2K(p_comp − 0.5)^2).
> 
> Our empirical results with the challenging MMLU-Pro benchmark validate the technical assumptions, as well as the efficacy of the proposed algorithm and the gains from scaling up its test-time compute.

N개 샘플을 생성한 다음 각 샘플의 페어를 K번 비교하는 토너먼트를 사용하는 Test Time Scaling 방법. 정답을 생성할 확률이 0보다 크고 비교에서 정답을 선택할 확률이 0.5보다 크다면 N과 K의 증가에 따라 오답률이 0으로 수렴한다는 이야기를 합니다.

<english>
Test time scaling method that uses tournament of N samples and K comparisons between each pair os samples. If probability of generating the correct answer is larger than 0 and choice the correct answer is larger than 0.5 then probability of inaccurate answer will be converge to 0 when N and K is increases.
</english>

#search 

