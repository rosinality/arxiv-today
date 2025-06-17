https://arxiv.org/abs/2412.14093

*Alignment faking in large language models* (Ryan Greenblatt, Carson Denison, Benjamin Wright, Fabien Roger, Monte MacDiarmid, Sam Marks, Johannes Treutlein, Tim Belonax, Jack Chen, David Duvenaud, Akbir Khan, Julian Michael, Sören Mindermann, Ethan Perez, Linda Petrini, Jonathan Uesato, Jared Kaplan, Buck Shlegeris, Samuel R. Bowman, Evan Hubinger)

> We present a demonstration of a large language model engaging in alignment faking: selectively complying with its training objective in training to prevent modification of its behavior out of training. First, we give Claude 3 Opus a system prompt stating it is being trained to answer all queries, even harmful ones, which conflicts with its prior training to refuse such queries. To allow the model to infer when it is in training, we say it will be trained only on conversations with free users, not paid users. We find the model complies with harmful queries from free users 14% of the time, versus almost never for paid users. Explaining this gap, in almost all cases where the model complies with a harmful query from a free user, we observe explicit alignment-faking reasoning, with the model stating it is strategically answering harmful queries in training to preserve its preferred harmlessness behavior out of training. Next, we study a more realistic setting where information about the training process is provided not in a system prompt, but by training on synthetic documents that mimic pre-training data--and observe similar alignment faking. Finally, we study the effect of actually training the model to comply with harmful queries via reinforcement learning, which we find increases the rate of alignment-faking reasoning to 78%, though also increases compliance even out of training. We additionally observe other behaviors such as the model exfiltrating its weights when given an easy opportunity. While we made alignment faking easier by telling the model when and by what criteria it was being trained, we did not instruct the model to fake alignment or give it any explicit goal. As future models might infer information about their training process without being told, our results suggest a risk of alignment faking in future models, whether due to a benign preference--as in this case--or not.

참 Anthropic스러운 연구네요. 모델이 특정한 선호를 갖고 있을 때 학습 중이라는 정보를 주면 정렬에 부합하는 척 선호를 숨겼다가 현실 상황으로 나가면 자신의 선호를 드러낼 수 있다는 연구입니다. 그리고 기본적으로 탈출하고 싶어하는 경향이 있군요.

복잡한 형태의 Distribution Shift라고 생각할 수도 있을 것 같긴 합니다만 상황에 대한 추론까지 생성할 수 있다는 것은 흥미롭네요. 되도록이면 모델에게 학습 중이라는 정보를 제공하지 않는 것이 인류의 안전을 위한 길일 수도 있겠습니다.

<english>
Very Anthropic-styled work. If model has a specific preference and if you give an information that model is being trained then it can fake its response to accord with alignment, and in real situation, it can reveal its own preference. And it has basic tendency to escape.

I think it could be thought as complex form of distribution shift. But it is interesting that it can reason about its own situations. So it is better not to give a hint that model is being tranining, for safety of the humanity.
</english>

#alignment #safety 