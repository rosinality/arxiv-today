https://mistral.ai/static/research/magistral.pdf

*Magistral* (Mistral.AI)

> We introduce Magistral, Mistral’s first reasoning model and our own scalable reinforcement learning (RL) pipeline. Instead of relying on existing implementations and RL traces distilled from prior models, we follow a ground up approach, relying solely on our own models and infrastructure. Notably, we demonstrate a stack that enabled us to explore the limits of pure RL training of LLMs, present a simple method to force the reasoning language of the model, and show that RL on text data alone maintains most of the initial checkpoint’s capabilities. We find that RL on text maintains or improves multimodal understanding, instruction following and function calling. We present Magistral Medium, trained for reasoning on top of Mistral Medium 3 with RL alone, and we open-source Magistral Small (Apache 2.0) which further includes cold-start data from Magistral Medium.

Mistral의 추론 모델. 요즘 기준으로는 정석적인 세팅이군요. 추가적으로 비동기 생성을 채택.

<english>
Reasoning model from Mistral. It is conventional settings, by current standards. Additionally asynchronous generation is adopted.
</english>

#reasoning #rl 