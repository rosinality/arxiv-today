https://arxiv.org/abs/2409.14586

*Backtracking Improves Generation Safety* (Yiming Zhang, Jianfeng Chi, Hailey Nguyen, Kartikeya Upasani, Daniel M. Bikel, Jason Weston, Eric Michael Smith)

> Text generation has a fundamental limitation almost by definition: there is no taking back tokens that have been generated, even when they are clearly problematic. In the context of language model safety, when a partial unsafe generation is produced, language models by their nature tend to happily keep on generating similarly unsafe additional text. This is in fact how safety alignment of frontier models gets circumvented in the wild, despite great efforts in improving their safety. Deviating from the paradigm of approaching safety alignment as prevention (decreasing the probability of harmful responses), we propose backtracking, a technique that allows language models to "undo" and recover from their own unsafe generation through the introduction of a special [RESET] token. Our method can be incorporated into either SFT or DPO training to optimize helpfulness and harmlessness. We show that models trained to backtrack are consistently safer than baseline models: backtracking Llama-3-8B is four times more safe than the baseline model (6.1\% $\to$ 1.5\%) in our evaluations without regression in helpfulness. Our method additionally provides protection against four adversarial attacks including an adaptive attack, despite not being trained to do so.

Backtracking으로 안전한 응답을 생성하도록 유도. 위험한 응답을 생성하다가 리셋한 다음 안전한 응답으로 고치도록 학습시키는 방법입니다.

Self Correction은 지금 최고의 화제이죠. 그런 측면에서 생각해볼 수 있겠네요.

#rlhf #safety 