https://arxiv.org/abs/2410.01920

*Step-by-Step Reasoning for Math Problems via Twisted Sequential Monte Carlo* (Shengyu Feng, Xiang Kong, Shuang Ma, Aonan Zhang, Dong Yin, Chong Wang, Ruoming Pang, Yiming Yang)

> Augmenting the multi-step reasoning abilities of Large Language Models (LLMs) has been a persistent challenge. Recently, verification has shown promise in improving solution consistency by evaluating generated outputs. However, current verification approaches suffer from sampling inefficiencies, requiring a large number of samples to achieve satisfactory performance. Additionally, training an effective verifier often depends on extensive process supervision, which is costly to acquire. In this paper, we address these limitations by introducing a novel verification method based on Twisted Sequential Monte Carlo (TSMC). TSMC sequentially refines its sampling effort to focus exploration on promising candidates, resulting in more efficient generation of high-quality solutions. We apply TSMC to LLMs by estimating the expected future rewards at partial solutions. This approach results in a more straightforward training target that eliminates the need for step-wise human annotations. We empirically demonstrate the advantages of our method across multiple math benchmarks, and also validate our theoretical analysis of both our approach and existing verification methods.

Majority Voting이나 Reward Model을 사용한 Verification을 Importance Sampling으로 해석한 다음 Importance Sampling의 샘플링 효율성을 높이기 위한 방법으로 Twisted Sequential Monte Carlo를 사용. (https://arxiv.org/abs/2404.17546) 유도를 쭉 따라가면 결과적으로 Value Function을 추정해서 활용하는 형태가 되는군요.

<english>
Interpret majority voting or verification using reward model as an importance sampling, and to improve sampling efficiency of importance sampling the paper have used twisted sequential monte carlo. (https://arxiv.org/abs/2404.17546) After following the derviation resulting algorithm is employ value function to do sampling.
</english>

#search

# Links

