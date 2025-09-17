https://arxiv.org/abs/2509.01440

*Benchmarking Optimizers for Large Language Model Pretraining* (Andrei Semenov, Matteo Pagliardini, Martin Jaggi)

> The recent development of Large Language Models (LLMs) has been accompanied by an effervescence of novel ideas and methods to better optimize the loss of deep learning models. Claims from those methods are myriad: from faster convergence to removing reliance on certain hyperparameters. However, the diverse experimental protocols used to validate these claims make direct comparisons between methods challenging. This study presents a comprehensive evaluation of recent optimization techniques across standardized LLM pretraining scenarios, systematically varying model size, batch size, and training duration. Through careful tuning of each method, we provide guidance to practitioners on which optimizer is best suited for each scenario. For researchers, our work highlights promising directions for future optimization research. Finally, by releasing our code and making all experiments fully reproducible, we hope our efforts can help the development and rigorous benchmarking of future methods.

Optimizer 벤치마크 1. AdEMAMix는 흥미로움. (최근에 쓰인 사례도 등장. https://github.com/swiss-ai/apertus-tech-report/blob/main/Apertus_Tech_Report.pdf) 유망한 Optimizer가 몇 있는데 토큰 효율성은 어느 정도일지?

Optimizer benchmarks 1. AdEMAMix is interesting. (It has been used in a recent model, https://github.com/swiss-ai/apertus-tech-report/blob/main/Apertus_Tech_Report.pdf) There are promising optimizers. How would they compare in token efficiency?

#optimizer 