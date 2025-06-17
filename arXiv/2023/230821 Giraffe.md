https://arxiv.org/abs/2308.10882

Giraffe: Adventurles in Expanding Context Lengths in LLMs (Arka Pal, Deep Karkhanis, Manley Roberts, Samuel Dooley, Arvind Sundararajan, Siddartha Naidu)

length extrapolation에 대한 결과 하나. 이쪽은 rope basis에 대해 truncation을 적용해 high frequency는 보존하고 low frequency를 clipping 해봤군요.

결과들이 복잡하긴 한데 perplexity를 보면 context length 2배 증가 정도를 기대할 수 있지 않나 싶습니다.

https://blog.abacus.ai/blog/2023/08/22/giraffe-long-context-llms/

개인적으로 GPT-4나 Claude 2에 대해서 가장 궁금한 점 중 하나가 대체 positional embedding으로 뭘 썼는가네요.