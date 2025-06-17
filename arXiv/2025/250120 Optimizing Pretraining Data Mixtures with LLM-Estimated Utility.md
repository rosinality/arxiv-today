https://arxiv.org/abs/2501.11747

*Optimizing Pretraining Data Mixtures with LLM-Estimated Utility* (William Held, Bhargavi Paranjape, Punit Singh Koura, Mike Lewis, Frank Zhang, Todor Mihaylov)

> Large Language Models improve with increasing amounts of high-quality training data. However, leveraging larger datasets requires balancing quality, quantity, and diversity across sources. After evaluating nine baseline methods under both compute- and data-constrained scenarios, we find token-count heuristics outperform manual and learned mixes, indicating that simple approaches accounting for dataset size and diversity are surprisingly effective. Building on this insight, we propose two complementary approaches: UtiliMax, which extends token-based heuristics by incorporating utility estimates from reduced-scale ablations, achieving up to a 10.6x speedup over manual baselines; and Model Estimated Data Utility (MEDU), which leverages LLMs to estimate data utility from small samples, matching ablation-based performance while reducing computational requirements by $\sim$200x. Together, these approaches establish a new framework for automated, compute-efficient data mixing that is robust across training regimes.

프리트레이닝 데이터셋 비율 결정 방법. 흥미롭게도 언어 비율 설정을 위해 개발된 방법인 UniMax가 (https://arxiv.org/abs/2304.09151) 꽤 좋은 방법이었다고 하네요. 그래서 UniMax에 평가 데이터셋에 대한 Loss를 Utility로 결합한 방법을 설계했습니다.

<english>
A method for determining dataset raio for pretraining. Interestingly UniMax which is developed for specifying language ratios was quite works well. Therefore they designed a method that combines loss of task datasets as an utility with UniMax.
</english>

#pretraining #dataset

# Links

[[230418 UniMax.md]]