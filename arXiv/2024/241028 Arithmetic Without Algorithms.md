https://arxiv.org/abs/2410.21272

*Arithmetic Without Algorithms: Language Models Solve Math With a Bag of Heuristics* (Yaniv Nikankin, Anja Reusch, Aaron Mueller, Yonatan Belinkov)

> Do large language models (LLMs) solve reasoning tasks by learning robust generalizable algorithms, or do they memorize training data? To investigate this question, we use arithmetic reasoning as a representative task. Using causal analysis, we identify a subset of the model (a circuit) that explains most of the model's behavior for basic arithmetic logic and examine its functionality. By zooming in on the level of individual circuit neurons, we discover a sparse set of important neurons that implement simple heuristics. Each heuristic identifies a numerical input pattern and outputs corresponding answers. We hypothesize that the combination of these heuristic neurons is the mechanism used to produce correct arithmetic answers. To test this, we categorize each neuron into several heuristic types-such as neurons that activate when an operand falls within a certain range-and find that the unordered combination of these heuristic types is the mechanism that explains most of the model's accuracy on arithmetic prompts. Finally, we demonstrate that this mechanism appears as the main source of arithmetic accuracy early in training. Overall, our experimental results across several LLMs show that LLMs perform arithmetic using neither robust algorithms nor memorization; rather, they rely on a "bag of heuristics".

LLM에서 계산이 값의 범위 체크 같은 휴리스틱의 결합으로 수행되는 것 같다는 분석.

<english>
Analysis that LLMs do arithmetic operations by combining heuristics like value bound checks.
</english>

#transformer #mechanistic-interpretation 