https://arxiv.org/abs/2404.10102

*Chinchilla Scaling: A replication attempt* (Tamay Besiroglu, Ege Erdil, Matthew Barnett, Josh You)

> Hoffmann et al. (2022) propose three methods for estimating a compute-optimal scaling law. We attempt to replicate their third estimation procedure, which involves fitting a parametric loss function to a reconstruction of data from their plots. We find that the reported estimates are inconsistent with their first two estimation methods, fail at fitting the extracted data, and report implausibly narrow confidence intervals--intervals this narrow would require over 600,000 experiments, while they likely only ran fewer than 500. In contrast, our rederivation of the scaling law using the third approach yields results that are compatible with the findings from the first two estimation procedures described by Hoffmann et al.

Chinchilla 논문의 SVG 이미지에서 값들을 뽑아 Chinchilla의 Parametric Function을 다시 추정해봤군요. 결과적으로 파라미터가 상당히 다르다고 합니다. Chinchilla의 Parameteric Fit으로 최적 파라미터와 데이터의 규모를 유도했을 때 다른 접근과 차이가 상당히 크다는 점에서 이상하다고 생각하는 사람들이 많았을 것 같은데, 다시 추정한 파라미터를 사용하면 1:20이라는 파라미터 대 데이터의 비율에 좀 더 가까운 값이 나오는군요.

#scaling-law 