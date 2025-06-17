https://arxiv.org/abs/2404.13208

*The Instruction Hierarchy: Training LLMs to Prioritize Privileged Instructions* (Eric Wallace, Kai Xiao, Reimar Leike, Lilian Weng, Johannes Heidecke, Alex Beutel)

> Today's LLMs are susceptible to prompt injections, jailbreaks, and other attacks that allow adversaries to overwrite a model's original instructions with their own malicious prompts. In this work, we argue that one of the primary vulnerabilities underlying these attacks is that LLMs often consider system prompts (e.g., text from an application developer) to be the same priority as text from untrusted users and third parties. To address this, we propose an instruction hierarchy that explicitly defines how models should behave when instructions of different priorities conflict. We then propose a data generation method to demonstrate this hierarchical instruction following behavior, which teaches LLMs to selectively ignore lower-privileged instructions. We apply this method to GPT-3.5, showing that it drastically increases robustness -- even for attack types not seen during training -- while imposing minimal degradations on standard capabilities.

Instruction의 위계를 모델에 부여하기 위한 방법. 예를 들어 시스템 메시지는 가장 우선해야 하고 모델 출력은 하위에 있어야 하죠. Anthropic의 Many-shot Jailbreaking도 생각나네요. (https://www.anthropic.com/research/many-shot-jailbreaking)

방법이 좀 흥미롭습니다. 일단 Aligned Instruction에 대해서는 복합적인 Instruction으로 생성한 다음 이를 쪼개서 시스템 프롬프트로 Instruction이 들어갔을 때와 분해한 Instruction을 서로 다른 위계에 배치했을 때의 출력 결과가 같게 만듭니다. Misaligned의 경우에는 제약 조건에 대한 시스템 프롬프트를 생성하고 이를 공격하기 위한 프롬프트를 생성한 다음 이 공격 프롬프트가 주어지지 않았을 때와 같은 결과가 나오게 하거나 제약 조건과 부합하는 프롬프트가 나올 때까지 생성한 결과로 학습시키는 형태입니다.

재미있네요. 중요한 결과일 것 같습니다. 더 나아가 모델 출력에 대해 Downweight 해서 모델의 스스로의 생성 결과에 대한 의존성을 낮추는 방향으로도 이을 수 있지 않을까 하는 생각이 듭니다.

#instruction-tuning #safety 