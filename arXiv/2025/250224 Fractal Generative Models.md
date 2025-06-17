https://arxiv.org/abs/2502.17437

*Fractal Generative Models* (Tianhong Li, Qinyi Sun, Lijie Fan, Kaiming He)

> Modularization is a cornerstone of computer science, abstracting complex functions into atomic building blocks. In this paper, we introduce a new level of modularization by abstracting generative models into atomic generative modules. Analogous to fractals in mathematics, our method constructs a new type of generative model by recursively invoking atomic generative modules, resulting in self-similar fractal architectures that we call fractal generative models. As a running example, we instantiate our fractal framework using autoregressive models as the atomic generative modules and examine it on the challenging task of pixel-by-pixel image generation, demonstrating strong performance in both likelihood estimation and generation quality. We hope this work could open a new paradigm in generative modeling and provide a fertile ground for future research. Code is available at https://github.com/LTH14/fractalgen.

시퀀스를 재귀적으로 쪼개고 쪼개진 시퀀스 내에서 Autoregressive 학습을 하는 모델이군요. 구현조차도 재귀적입니다.

<english>
Generative model that recursively splits a sequence and autoregressively trained on splitted sequence. Implementation itself also recursive.
</english>

#generative-model #autoregressive-model 