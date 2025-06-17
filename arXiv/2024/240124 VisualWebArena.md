https://arxiv.org/abs/2401.13649

*VisualWebArena: Evaluating Multimodal Agents on Realistic Visual Web Tasks* (Jing Yu Koh, Robert Lo, Lawrence Jang, Vikram Duvvur, Ming Chong Lim, Po-Yu Huang, Graham Neubig, Shuyan Zhou, Ruslan Salakhutdinov, Daniel Fried)

> Autonomous agents capable of planning, reasoning, and executing actions on the web offer a promising avenue for automating computer tasks. However, the majority of existing benchmarks primarily focus on text-based agents, neglecting many natural tasks that require visual information to effectively solve. Given that most computer interfaces cater to human perception, visual information often augments textual data in ways that text-only models struggle to harness effectively. To bridge this gap, we introduce VisualWebArena, a benchmark designed to assess the performance of multimodal web agents on realistic \textit{visually grounded tasks}. VisualWebArena comprises of a set of diverse and complex web-based tasks that evaluate various capabilities of autonomous multimodal agents. To perform on this benchmark, agents need to accurately process image-text inputs, interpret natural language instructions, and execute actions on websites to accomplish user-defined objectives. We conduct an extensive evaluation of state-of-the-art LLM-based autonomous agents, including several multimodal models. Through extensive quantitative and qualitative analysis, we identify several limitations of text-only LLM agents, and reveal gaps in the capabilities of state-of-the-art multimodal language agents. VisualWebArena provides a framework for evaluating multimodal autonomous language agents, and offers insights towards building stronger autonomous agents for the web. Our code, baseline models, and data is publicly available at https://jykoh.com/vwa.

https://jykoh.com/vwa

웹사이트를 대상으로 한 Agent로서의 능력을 평가하는 벤치마크. 웹사이트가 변화하면 안 되니 웹사이트를 독립적으로 만들어서 띄울 수 있게 했군요.

웹이나 모바일 앱을 대상으로 하는 Agent 모델들에 대한 관심이 꽤 있는 것 같습니다. 얼마나 실용적으로 유용할지는 잘 모르겠지만 (https://x.com/astralwave/status/1744968755565023437) 모델의 능력을 테스트하기에는 흥미롭지 않나 싶습니다.

#benchmark #agent 