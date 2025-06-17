https://arxiv.org/abs/2412.04403

*Establishing Task Scaling Laws via Compute-Efficient Model Ladders* (Akshita Bhagia, Jiacheng Liu, Alexander Wettig, David Heineman, Oyvind Tafjord, Ananya Harsh Jha, Luca Soldaini, Noah A. Smith, Dirk Groeneveld, Pang Wei Koh, Jesse Dodge, Hannaneh Hajishirzi)

> We develop task scaling laws and model ladders to predict the individual task performance of pretrained language models (LMs) in the overtrained setting. Standard power laws for language modeling loss cannot accurately model task performance. Therefore, we leverage a two-step prediction approach: first use model and data size to predict a task-specific loss, and then use this task loss to predict task performance. We train a set of small-scale "ladder" models, collect data points to fit the parameterized functions of the two prediction steps, and make predictions for two target models: a 7B model trained to 4T tokens and a 13B model trained to 5T tokens. Training the ladder models only costs 1% of the compute used for the target models. On four multiple-choice tasks written in ranked classification format, we can predict the accuracy of both target models within 2 points of absolute error. We have higher prediction error on four other tasks (average absolute error 6.9) and find that these are often tasks with higher variance in task metrics. We also find that using less compute to train fewer ladder models tends to deteriorate predictions. Finally, we empirically show that our design choices and the two-step approach lead to superior performance in establishing scaling laws.

위의 연구와 (https://arxiv.org/abs/2412.04315) 비슷하게 Llama 3 스타일의 Task Loss 예측과 Loss를 통한 Accuracy 예측을 결합한 Task Scaling Law를 시도했군요. 예측이 성공적이네요. 이 접근이 Task Scaling Law에 대해서는 상당히 괜찮은 것 같습니다.

<english>
Similar to above study (https://arxiv.org/abs/2412.04315) the authors tried to estimate Llama 3 style task scaling law which combines task loss prediction and accuracy prediction using the loss. Prediction was successful. It seems that this approach works well for estimation of task scaling law.
</english>

#scaling-law

# Links

[[241205 Densing Law of LLMs.md]]