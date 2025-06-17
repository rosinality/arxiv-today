https://arxiv.org/abs/2410.15466

*Keep Guessing? When Considering Inference Scaling, Mind the Baselines* (Gal Yona, Or Honovich, Omer Levy, Roee Aharoni)

> Scaling inference compute in large language models (LLMs) through repeated sampling consistently increases the coverage (fraction of problems solved) as the number of samples increases. We conjecture that this observed improvement is partially due to the answer distribution of standard evaluation benchmarks, which is skewed towards a relatively small set of common answers. To test this conjecture, we define a baseline that enumerates answers according to their prevalence in the training set. Experiments spanning two domains -- mathematical reasoning and factual knowledge -- reveal that this baseline outperforms repeated model sampling for some LLMs, while the coverage for others is on par with that of a mixture strategy that obtains $k$ answers by using only $10$ model samples and similarly guessing the remaining $k-10$ attempts via enumeration. Our baseline enables a more accurate measurement of how much repeated sampling improves coverage in such settings beyond prompt-agnostic guessing.

Inference Scaling을 측정할 때 학습 셋에 자주 등장한 Top K개의 정답을 사용하는 베이스라인으로 보정해야 한다는 주장. 굉장히 중요한 지적 같네요.

<english>
The suggestion that you should adjust inference scaling with baseline that uses most frequent answers from the training set. I think this is very important point
</english>

#search 