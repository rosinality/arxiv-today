https://arxiv.org/abs/2402.01035

*Getting the most out of your tokenizer for pre-training and domain adaptation* (Gautier Dagan, Gabriele Synnaeve, Baptiste Rozière)

> Tokenization is an understudied and often neglected component of modern LLMs. Most published works use a single tokenizer for all experiments, often borrowed from another model, without performing ablations or analysis to optimize tokenization. Moreover, the tokenizer is generally kept unchanged when fine-tuning a base model. In this paper, we show that the size, pre-tokenization regular expression, and training data of a tokenizer can significantly impact the model's generation speed, effective context size, memory usage, and downstream performance. We train specialized Byte-Pair Encoding code tokenizers, and conduct extensive ablations on the impact of tokenizer design on the performance of LLMs for code generation tasks such as HumanEval and MBPP, and provide recommendations for tokenizer hyper-parameters selection and switching the tokenizer in a pre-trained LLM. We perform our experiments on models trained from scratch and from pre-trained models, verifying their applicability to a wide range of use-cases. We find that when fine-tuning on more than 50 billion tokens, we can specialize the tokenizer of a pre-trained LLM to obtain large gains in generation speed and effective context size.

Llama에서 Code Llama로 넘어갔을 때 토크나이저를 바꿨다면 어땠을까? 하는 질문. 토크나이저의 학습 분포를 바꾸는 것과 PreTokenizer를 바꾸는 것을 모두 고려합니다.

결론은 충분한 데이터(아마도 50B 이상)를 쓴다면 토크나이저를 바꾸는 것이 문제가 없을 것 같다는 것입니다. 토크나이저를 바꿨다면 효율성을 같이 가져갔을 수 있지 않았을까 하는 결론이군요.

#tokenizer #finetuning 

How would it perform if we changed tokenizer of Llama during the process of finetuning it to build Code Llama? This study considers changing distribution of tokenizer training and replacing pre-tokenizers.

Conclusion is that if we use enough data to finetuning it (maybe above 50B) then it is not problematic to change the tokenizer. We can think if tokenizer changed then we would got better inference efficiency without compromising the performance.