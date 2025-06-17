https://arxiv.org/abs/2504.19110

*APE-Bench I: Towards File-level Automated Proof Engineering of Formal Math Libraries* (Huajian Xin, Luming Li, Xiaoran Jin, Jacques Fleuriot, Wenda Li)

> Recent progress in large language models (LLMs) has shown promise in formal theorem proving, yet existing benchmarks remain limited to isolated, static proof tasks, failing to capture the iterative, engineering-intensive workflows of real-world formal mathematics libraries. Motivated by analogous advances in software engineering, we introduce the paradigm of Automated Proof Engineering (APE), which aims to automate proof engineering tasks such as feature addition, proof refactoring, and bug fixing using LLMs. To facilitate research in this direction, we present APE-Bench I, the first realistic benchmark built from real-world commit histories of Mathlib4, featuring diverse file-level tasks described in natural language and verified via a hybrid approach combining the Lean compiler and LLM-as-a-Judge. We further develop Eleanstic, a scalable parallel verification infrastructure optimized for proof checking across multiple versions of Mathlib. Empirical results on state-of-the-art LLMs demonstrate strong performance on localized edits but substantial degradation on handling complex proof engineering. This work lays the foundation for developing agentic workflows in proof engineering, with future benchmarks targeting multi-file coordination, project-scale verification, and autonomous agents capable of planning, editing, and repairing formal libraries.

Proof Assistant로 증명을 하는 것을 넘어 라이브러리 단위에서 작업하는 능력을 평가하는 벤치마크군요.

<english>
Beyond proving using proof assistant, benchmark that evaluates capability of doing an work on the level of library has appeared.
</english>

#math #benchmark 