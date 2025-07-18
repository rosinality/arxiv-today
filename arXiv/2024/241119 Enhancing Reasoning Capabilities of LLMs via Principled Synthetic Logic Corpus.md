https://arxiv.org/abs/2411.12498

*Enhancing Reasoning Capabilities of LLMs via Principled Synthetic Logic Corpus* (Terufumi Morishita, Gaku Morio, Atsuki Yamaguchi, Yasuhiro Sogawa)

> Large language models (LLMs) are capable of solving a wide range of tasks, yet they have struggled with reasoning. To address this, we propose $\textbf{Additional Logic Training (ALT)}$, which aims to enhance LLMs' reasoning capabilities by program-generated logical reasoning samples. We first establish principles for designing high-quality samples by integrating symbolic logic theory and previous empirical insights. Then, based on these principles, we construct a synthetic corpus named $\textbf{Formal Logic Deduction Diverse}$ ($\textbf{FLD}$$^{\times 2}$), comprising numerous samples of multi-step deduction with unknown facts, diverse reasoning rules, diverse linguistic expressions, and challenging distractors. Finally, we empirically show that ALT on FLD$^{\times2}$ substantially enhances the reasoning capabilities of state-of-the-art LLMs, including LLaMA-3.1-70B. Improvements include gains of up to 30 points on logical reasoning benchmarks, up to 10 points on math and coding benchmarks, and 5 points on the benchmark suite BBH.

논리 추론 데이터를 생성해서 모델을 학습시킨다는 아이디어.

<english>
Training model using synthesized logical reasoning data.
</english>

#reasoning #synthetic-data 