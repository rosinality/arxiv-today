https://arxiv.org/abs/2406.19292

*From Artificial Needles to Real Haystacks: Improving Retrieval Capabilities in LLMs by Finetuning on Synthetic Data* (Zheyang Xiong, Vasilis Papageorgiou, Kangwook Lee, Dimitris Papailiopoulos)

> Recent studies have shown that Large Language Models (LLMs) struggle to accurately retrieve information and maintain reasoning capabilities when processing long-context inputs. To address these limitations, we propose a finetuning approach utilizing a carefully designed synthetic dataset comprising numerical key-value retrieval tasks. Our experiments on models like GPT-3.5 Turbo and Mistral 7B demonstrate that finetuning LLMs on this dataset significantly improves LLMs' information retrieval and reasoning capabilities in longer-context settings. We present an analysis of the finetuned models, illustrating the transfer of skills from synthetic to real task evaluations (e.g., $10.5\%$ improvement on $20$ documents MDQA at position $10$ for GPT-3.5 Turbo). We also find that finetuned LLMs' performance on general benchmarks remains almost constant while LLMs finetuned on other baseline long-context augmentation data can encourage hallucination (e.g., on TriviaQA, Mistral 7B finetuned on our synthetic data cause no performance drop while other baseline data can cause a drop that ranges from $2.33\%$ to $6.19\%$). Our study highlights the potential of finetuning on synthetic data for improving the performance of LLMs on longer-context tasks.

Dictionary에 대한 Key-Value Retrieval 같은 순수하게 인공적인 과제로도 Long Context QA 같은 과제에 대한 성능을 높여줄 수 있다는 결과. 얼마 전 텍스트에서 이미지로, 이미지에서 비디오로 Long Context 능력을 일반화한 경우도 그렇고 (https://arxiv.org/abs/2406.16852) Long Context 능력은 일반화가 굉장히 잘 일어나는 문제인 것 같기도 합니다.

답변 형식을 프롬프트에 추가해서 특정한 답변 형식을 학습하지 않도록 방지한 것, Long Context QA를 인위적으로 구성해서 학습하는 것보다 할루시네이션의 가능성을 억제할 수도 있다는 가능성 등의 측면에서 말끔한 접근이라는 느낌입니다.

#long-context

# Links

[[240624 Long Context Transfer from Language to Vision.md]]