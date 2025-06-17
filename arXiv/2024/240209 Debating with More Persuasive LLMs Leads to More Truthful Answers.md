https://arxiv.org/abs/2402.06782

*Debating with More Persuasive LLMs Leads to More Truthful Answers* (Akbir Khan, John Hughes, Dan Valentine, Laura Ruis, Kshitij Sachan, Ansh Radhakrishnan, Edward Grefenstette, Samuel R. Bowman, Tim Rocktäschel, Ethan Perez)

> Common methods for aligning large language models (LLMs) with desired behaviour heavily rely on human-labelled data. However, as models grow increasingly sophisticated, they will surpass human expertise, and the role of human evaluation will evolve into non-experts overseeing experts. In anticipation of this, we ask: can weaker models assess the correctness of stronger models? We investigate this question in an analogous setting, where stronger models (experts) possess the necessary information to answer questions and weaker models (non-experts) lack this information. The method we evaluate is \textit{debate}, where two LLM experts each argue for a different answer, and a non-expert selects the answer. We find that debate consistently helps both non-expert models and humans answer questions, achieving 76\% and 88\% accuracy respectively (naive baselines obtain 48\% and 60\%). Furthermore, optimising expert debaters for persuasiveness in an unsupervised manner improves non-expert ability to identify the truth in debates. Our results provide encouraging empirical evidence for the viability of aligning models with debate in the absence of ground truth.

Weak-to-Strong Generalization 문제. 여기서의 특징은 능력이 아니라 정보의 측면에서 Weak와 Strong을 구분했다는 것이네요. Strong에서는 답에 대한 맥락 정보를 접근할 수 있고 Weak는 그 정보에 접근할 수 없습니다. 여기서의 제안 방법은 Strong 모델들이 논쟁을 하게 하고, 논쟁 과정에서 설득력이 높아지도록 했을 때 Weak 모델의 판단 정확도가 높아졌다는 결과입니다.

능력이 아니라 정보의 비대칭성을 고려하는 것이고, 인용 도구를 사용해서 Strong 모델이 텍스트를 직접 넘겨줄 수 있고 인용 텍스트를 검증할 수 있었다는 점에서 제한적이긴 합니다. 전문가들끼리 논쟁시킨 다음 더 설득력이 있는 것을 정답이라고 하면 맞을 가능성이 높을 것이다...라는 아이디어는 매력적이지만요.

#alignment

Weak-to-Strong Generalization Problem. In this scenario asymmetry is assumed between in informations, not capabilities. Strong models has access to privileged informations that context for solutions, and weak models does not has it. This study suggests method that make strong models to debate, and if we optimize to increase persuasiveness of debate, then judge accuracy of weak model is enhanced.

Limitation of this study is that it only considers asymmetry in informations, not capabilities, and strong models can use quote tool to extract texts from inputs, and it is possible to verify correctness of quoted texts. The idea that make experts debating and choose the most persuasive answer is attractive, though.