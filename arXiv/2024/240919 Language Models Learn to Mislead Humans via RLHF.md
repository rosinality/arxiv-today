https://arxiv.org/abs/2409.12822

*Language Models Learn to Mislead Humans via RLHF* (Jiaxin Wen, Ruiqi Zhong, Akbir Khan, Ethan Perez, Jacob Steinhardt, Minlie Huang, Samuel R. Boman, He He, Shi Feng)

> Language models (LMs) can produce errors that are hard to detect for humans, especially when the task is complex. RLHF, the most popular post-training method, may exacerbate this problem: to achieve higher rewards, LMs might get better at convincing humans that they are right even when they are wrong. We study this phenomenon under a standard RLHF pipeline, calling it "U-SOPHISTRY" since it is Unintended by model developers. Specifically, we ask time-constrained (e.g., 3-10 minutes) human subjects to evaluate the correctness of model outputs and calculate humans' accuracy against gold labels. On a question-answering task (QuALITY) and programming task (APPS), RLHF makes LMs better at convincing our subjects but not at completing the task correctly. RLHF also makes the model harder to evaluate: our subjects' false positive rate increases by 24.1% on QuALITY and 18.3% on APPS. Finally, we show that probing, a state-of-the-art approach for detecting Intended Sophistry (e.g. backdoored LMs), does not generalize to U-SOPHISTRY. Our results highlight an important failure mode of RLHF and call for more research in assisting humans to align them.

RLHF를 거치면서 모델이 실제 성능은 높아지지 않으면서 사람에 대한 설득력은 높아져 사람의 평가는 높일 수 있다는 결과. 사람이 작성한 유닛 테스트에도 비슷한 현상이 일어날 수 있습니다. 사람에 대해서 Reward Hacking을 했다고 할 수 있겠네요.

Alignment 연구자들이 가장 두려워하는 주제라 혹시 싶었는데 아니나 다를까 Anthropic 저자들이 들어가 있네요.

#alignment #safety 