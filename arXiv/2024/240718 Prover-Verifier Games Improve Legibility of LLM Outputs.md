https://cdn.openai.com/prover-verifier-games-improve-legibility-of-llm-outputs/legibility.pdf

*Prover-Verifier Games Improve Legibility of LLM Outputs* (Jan Hendrik Kirchner, Yining CHen, harri Edwards, Jan Leike, Nat McAleese, Yuri Burda)

> One way to increase confidence in the outputs of Large Language Models (LLMs) is to support them with reasoning that is clear and easy to check — a property we call legibility. We study legibility in the context of solving grade-school math problems and show that optimizing chain-of-thought solutions only for answer correctness can make them less legible. To mitigate the loss in legibility, we propose a training algorithm inspired by Prover-Verifier Game from Anil et al. (2021). Our algorithm iteratively trains small verifiers to predict solution correctness, “helpful” provers to produce correct solutions that the verifier accepts, and “sneaky” provers to produce incorrect solutions that fool the verifier. We find that the helpful prover’s accuracy and the verifier’s robustness to adversarial attacks increase over the course of training. Furthermore, we show that legibility training transfers to time-constrained humans tasked with verifying solution correctness. Over course of LLM training human accuracy increases when checking the helpful prover’s solutions, and decreases when checking the sneaky prover’s solutions. Hence, training for checkability by small verifiers is a plausible technique for increasing output legibility. Our results suggest legibility training against small verifiers as a practical avenue for increasing legibility of large LLMs to humans, and thus could help with alignment of superhuman models.

LLM이 사람이 이해하기 쉬운 결과를 생성하도록 학습할 수 있는가 하는 문제. 초지능이 답변을 해주는데 사람은 이해하지 못하는 상황을 상상한 것이 아닌가 싶네요.

GSM 데이터셋을 기반으로 했는데 아이디어는 이렇습니다. Prover와 Verifier라는 두 모델을 두고 Verifier는 Prover의 결과가 정답인지 아닌지를 판단합니다. Prover는 Helpful 모드에서는 정답을 생성하고 Sneaky 모드일 때는 오답을 생성하면서 Verifier에게는 정답이라고 판단되도록 합니다. Verifier는 정답을 구분하도록 학습합니다.  이를 통해 Helpful 모드일 때는 좀좀 더 이해하기 쉬운 답을 생성하도록 학습되었다고 하네요.

(역설적이지만 결과적으로 Sneaky 모드일 때는 점점 더 판단하기 어려운 답을 생성하게 되는군요.)

#safety #alignment 