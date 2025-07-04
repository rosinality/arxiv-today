https://arxiv.org/abs/2507.02856

*Answer Matching Outperforms Multiple Choice for Language Model Evaluation* (Nikhil Chandak, Shashwat Goel, Ameya Prabhu, Moritz Hardt, Jonas Geiping)

> Multiple choice benchmarks have long been the workhorse of language model evaluation because grading multiple choice is objective and easy to automate. However, we show multiple choice questions from popular benchmarks can often be answered without even seeing the question. These shortcuts arise from a fundamental limitation of discriminative evaluation not shared by evaluations of the model's free-form, generative answers. Until recently, there appeared to be no viable, scalable alternative to multiple choice--but, we show that this has changed. We consider generative evaluation via what we call answer matching: Give the candidate model the question without the options, have it generate a free-form response, then use a modern language model with the reference answer to determine if the response matches the reference. To compare the validity of different evaluation strategies, we annotate MMLU-Pro and GPQA-Diamond to obtain human grading data, and measure the agreement of each evaluation approach. We find answer matching using recent models--even small ones--achieves near-perfect agreement, in the range of inter-annotator agreement. In contrast, both multiple choice evaluation and using LLM-as-a-judge without reference answers aligns poorly with human grading. Improving evaluations via answer matching is not merely a conceptual concern: the rankings of several models change significantly when evaluating their free-form responses with answer matching. In light of these findings, we discuss how to move the evaluation ecosystem from multiple choice to answer matching.

MCQ 벤치마크에서 선택지를 제외하고 정답을 생성하게 한 다음 LLM으로 검증. 벤치마크의 난이도도 높아지고 좀 더 실용적인 척도라는 점에서 쓸만하겠네요.

<english>
Remove choices from MCQ benchmarks and let model to generate answer, and then verify it with LLM. It could be useful as it increases difficulty of the benchmarks and at the same time it would be a metric that reflects practical applications more well.
</english>

#benchmark 