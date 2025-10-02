https://arxiv.org/abs/2509.23045

*Kimi-Dev: Agentless Training as Skill Prior for SWE-Agents* (Zonghan Yang, Shengjie Wang, Kelin Fu, Wenyang He, Weimin Xiong, Yibo Liu, Yibo Miao, Bofei Gao, Yejie Wang, Yingwei Ma, Yanhao Li, Yue Liu, Zhenxing Hu, Kaitai Zhang, Shuyi Wang, Huarong Chen, Flood Sung, Yang Liu, Yang Gao, Zhilin Yang, Tianyu Liu)

> Large Language Models (LLMs) are increasingly applied to software engineering (SWE), with SWE-bench as a key benchmark. Solutions are split into SWE-Agent frameworks with multi-turn interactions and workflow-based Agentless methods with single-turn verifiable steps. We argue these paradigms are not mutually exclusive: reasoning-intensive Agentless training induces skill priors, including localization, code edit, and self-reflection that enable efficient and effective SWE-Agent adaptation. In this work, we first curate the Agentless training recipe and present Kimi-Dev, an open-source SWE LLM achieving 60.4\% on SWE-bench Verified, the best among workflow approaches. With additional SFT adaptation on 5k publicly-available trajectories, Kimi-Dev powers SWE-Agents to 48.6\% pass@1, on par with that of Claude 3.5 Sonnet (241022 version). These results show that structured skill priors from Agentless training can bridge workflow and agentic frameworks for transferable coding agents.

버그 고치기나 테스트 작성 같은 비에이전트 싱글 턴 능력에 대해 모델을 학습시켜서 에이전트 능력에 대한 기반으로 사용. 조합되었을 때의 더 나은 결과를 위해 개별 능력을 증진시키는 것은 자연스러운 일이지만, 환경이 스케일링 되는 것에 따라 과제들을 어떻게 분해할 수 있는가는 문제가 될 듯.

Training the model on agentless single-turn abilities like bug fixing or test writing to use as a foundation for agent capabilities. Enhancing individual abilities for better results when combined is natural, bu how tasks can be decomposed as environments scale?

#rl #agent #synthetic-data 