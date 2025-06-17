https://arxiv.org/abs/2505.05410

*Reasoning Models Don't Always Say What They Think* (Yanda Chen, Joe Benton, Ansh Radhakrishnan, Jonathan Uesato, Carson Denison, John Schulman, Arushi Somani, Peter Hase, Misha Wagner, Fabien Roger, Vlad Mikulik, Samuel R. Bowman, Jan Leike, Jared Kaplan, Ethan Perez)

> Chain-of-thought (CoT) offers a potential boon for AI safety as it allows monitoring a model's CoT to try to understand its intentions and reasoning processes. However, the effectiveness of such monitoring hinges on CoTs faithfully representing models' actual reasoning processes. We evaluate CoT faithfulness of state-of-the-art reasoning models across 6 reasoning hints presented in the prompts and find: (1) for most settings and models tested, CoTs reveal their usage of hints in at least 1% of examples where they use the hint, but the reveal rate is often below 20%, (2) outcome-based reinforcement learning initially improves faithfulness but plateaus without saturating, and (3) when reinforcement learning increases how frequently hints are used (reward hacking), the propensity to verbalize them does not increase, even without training against a CoT monitor. These results suggest that CoT monitoring is a promising way of noticing undesired behaviors during training and evaluations, but that it is not sufficient to rule them out. They also suggest that in settings like ours where CoT reasoning is not necessary, test-time monitoring of CoTs is unlikely to reliably catch rare and catastrophic unexpected behaviors.

추론 모델의 추론 과정이 실제로 일어나는 일을 충실히 반영하는 것은 아니라는 분석. 따라서 모델이 Reward Hacking을 하는 경우에도 추론 과정을 통해서 그걸 잡아내기는 어렵죠.

OpenAI도 비슷한 문제를 태클하면서 동시에 추론을 규율하는 것은 어렵다는 이야기를 했죠. (https://openai.com/index/chain-of-thought-monitoring/) 아는 것과 행동을 구분하는 것처럼 생각과 응답을 구분하는 것도 자연스러운 것이 아닐까요.

<english>
An analysis that reasoning from reasoning model is not faithfully reflects what is actually happening. Thus even when model doing reward hacking it is hard to catch it from reasoning process.

OpenAI tackled similar problems and also suggested it is hard to regularize the reasoning (https://openai.com/index/chain-of-thought-monitoring/). As it is natural to separate what model know and what model behaves, maybe separating thinkings and responses is natural thing to do.
</english>

#reasoning #reward 