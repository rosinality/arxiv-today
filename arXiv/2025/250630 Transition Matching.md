https://arxiv.org/abs/2506.23589

*Transition Matching: Scalable and Flexible Generative Modeling* (Neta Shaul, Uriel Singer, Itai Gat, Yaron Lipman)

> Diffusion and flow matching models have significantly advanced media generation, yet their design space is well-explored, somewhat limiting further improvements. Concurrently, autoregressive (AR) models, particularly those generating continuous tokens, have emerged as a promising direction for unifying text and media generation. This paper introduces Transition Matching (TM), a novel discrete-time, continuous-state generative paradigm that unifies and advances both diffusion/flow models and continuous AR generation. TM decomposes complex generation tasks into simpler Markov transitions, allowing for expressive non-deterministic probability transition kernels and arbitrary non-continuous supervision processes, thereby unlocking new flexible design avenues. We explore these choices through three TM variants: (i) Difference Transition Matching (DTM), which generalizes flow matching to discrete-time by directly learning transition probabilities, yielding state-of-the-art image quality and text adherence as well as improved sampling efficiency. (ii) Autoregressive Transition Matching (ARTM) and (iii) Full History Transition Matching (FHTM) are partially and fully causal models, respectively, that generalize continuous AR methods. They achieve continuous causal AR generation quality comparable to non-causal approaches and potentially enable seamless integration with existing AR text generation techniques. Notably, FHTM is the first fully causal model to match or surpass the performance of flow-based methods on text-to-image task in continuous domains. We demonstrate these contributions through a rigorous large-scale comparison of TM variants and relevant baselines, maintaining a fixed architecture, training data, and hyperparameters.

Diffusion 모델의 일반화. 마르코프 과정의 Transition Kernel로 더 다양한 커널을 사용할 수 있게 하는 형태군요. 이 커널로 Autoregressive 모델을 사용해서 Autoregressive 모델을 만들었군요.

<english>
A generalization of diffusion model. It is the form of allow more diverse kernels for transition kernels in markov process. They build autoregressive model by using autoregressive model as a kernel.
</english>

#diffusion #autoregressive-model 