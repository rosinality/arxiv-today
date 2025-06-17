https://arxiv.org/abs/2403.06634

*Stealing Part of a Production Language Model* (Nicholas Carlini, Daniel Paleka, Krishnamurthy Dj Dvijotham, Thomas Steinke, Jonathan Hayase, A. Feder Cooper, Katherine Lee, Matthew Jagielski, Milad Nasr, Arthur Conmy, Eric Wallace, David Rolnick, Florian Tramèr)

> We introduce the first model-stealing attack that extracts precise, nontrivial information from black-box production language models like OpenAI's ChatGPT or Google's PaLM-2. Specifically, our attack recovers the embedding projection layer (up to symmetries) of a transformer model, given typical API access. For under \$20 USD, our attack extracts the entire projection matrix of OpenAI's Ada and Babbage language models. We thereby confirm, for the first time, that these black-box models have a hidden dimension of 1024 and 2048, respectively. We also recover the exact hidden dimension size of the gpt-3.5-turbo model, and estimate it would cost under \$2,000 in queries to recover the entire projection matrix. We conclude with potential defenses and mitigations, and discuss the implications of possible future work that could extend our attack.

API로 모델 차원 크기와 임베딩 가중치를 뽑아내는 방법. Log Prob와 Logit Bias를 사용하면 효율적으로 공격할 수 있습니다. 그래서 OpenAI가 최근에 Logit Bias가 Log Prob에 영향을 미치지 않도록 수정했군요. (모델 차원 크기와 임베딩 가중치 정도는 알려줘도 되지 않을까 싶긴 합니다만.)

#attack 