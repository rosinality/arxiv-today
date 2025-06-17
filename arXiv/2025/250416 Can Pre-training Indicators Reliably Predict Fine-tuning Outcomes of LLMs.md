https://arxiv.org/abs/2504.12491

*Can Pre-training Indicators Reliably Predict Fine-tuning Outcomes of LLMs?* (Hansi Zeng, Kai Hui, Honglei Zhuang, Zhen Qin, Zhenrui Yue, Hamed Zamani, Dana Alon)

> While metrics available during pre-training, such as perplexity, correlate well with model performance at scaling-laws studies, their predictive capacities at a fixed model size remain unclear, hindering effective model selection and development. To address this gap, we formulate the task of selecting pre-training checkpoints to maximize downstream fine-tuning performance as a pairwise classification problem: predicting which of two LLMs, differing in their pre-training, will perform better after supervised fine-tuning (SFT). We construct a dataset using 50 1B parameter LLM variants with systematically varied pre-training configurations, e.g., objectives or data, and evaluate them on diverse downstream tasks after SFT. We first conduct a study and demonstrate that the conventional perplexity is a misleading indicator. As such, we introduce novel unsupervised and supervised proxy metrics derived from pre-training that successfully reduce the relative performance prediction error rate by over 50%. Despite the inherent complexity of this task, we demonstrate the practical utility of our proposed proxies in specific scenarios, paving the way for more efficient design of pre-training schemes optimized for various downstream tasks.

다양한 세팅으로 프리트레이닝된 LLM이 SFT를 거쳤을 때 어느 쪽이 나을지를 예측하려한 시도. UL2 같은 학습 Objective의 차이도 테스트했네요.

<english>
An attempt to predict which pretraining setting would be better after SFT. They also tested differences in training objectives like UL2.
</english>

#pretraining 