https://arxiv.org/abs/2502.17262

*Unveiling Downstream Performance Scaling of LLMs: A Clustering-Based Perspective* (Chengyin Xu, Kaiyuan Chen, Xiao Li, Ke Shen, Chenggang Li)

> The rapid advancements in computing dramatically increase the scale and cost of training Large Language Models (LLMs). Accurately predicting downstream task performance prior to model training is crucial for efficient resource allocation, yet remains challenging due to two primary constraints: (1) the "emergence phenomenon", wherein downstream performance metrics become meaningful only after extensive training, which limits the ability to use smaller models for prediction; (2) Uneven task difficulty distributions and the absence of consistent scaling laws, resulting in substantial metric variability. Existing performance prediction methods suffer from limited accuracy and reliability, thereby impeding the assessment of potential LLM capabilities. To address these challenges, we propose a Clustering-On-Difficulty (COD) downstream performance prediction framework. COD first constructs a predictable support subset by clustering tasks based on difficulty features, strategically excluding non-emergent and non-scalable clusters. The scores on the selected subset serve as effective intermediate predictors of downstream performance on the full evaluation set. With theoretical support, we derive a mapping function that transforms performance metrics from the predictable subset to the full evaluation set, thereby ensuring accurate extrapolation of LLM downstream performance. The proposed method has been applied to predict performance scaling for a 70B LLM, providing actionable insights for training resource allocation and assisting in monitoring the training process. Notably, COD achieves remarkable predictive accuracy on the 70B LLM by leveraging an ensemble of small models, demonstrating an absolute mean deviation of 1.36% across eight important LLM evaluation benchmarks.

Task Scaling Law. 클러스터링으로 난이도가 비슷한 문제들을 묶은 다음 예측이 잘 되는 샘플들을 선택하고 이 샘플들에 대한 예측을 기반으로 벤치마크 전체에 대한 예측을 하는 형태군요.

<english>
A task scaling law. They collect problems with similar difficulties using clustering and then select samples that can be easily predicted. Then doing a prediction on total benchmark samples based on the prediction for this subset.
</english>

#scaling-law 