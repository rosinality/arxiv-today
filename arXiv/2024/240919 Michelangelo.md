https://arxiv.org/abs/2409.12640

*Michelangelo: Long Context Evaluations Beyond Haystacks via Latent Structure Queries* (Kiran Vodrahalli, Santiago Ontanon, Nilesh Tripuraneni, Kelvin Xu, Sanil Jain, Rakesh Shivanna, Jeffrey Hui, Nishanth Dikkala, Mehran Kazemi, Bahare Fatemi, Rohan Anil, Ethan Dyer, Siamak Shakeri, Roopali Vij, Harsh Mehta, Vinay Ramasesh, Quoc Le, Ed Chi, Yifeng Lu, Orhan Firat, Angeliki Lazaridou, Jean-Baptiste Lespiau, Nithya Attaluri, Kate Olszewska)

> We introduce Michelangelo: a minimal, synthetic, and unleaked long-context reasoning evaluation for large language models which is also easy to automatically score. This evaluation is derived via a novel, unifying framework for evaluations over arbitrarily long contexts which measure the model's ability to do more than retrieve a single piece of information from its context. The central idea of the \frameworkname framework (\frameworkshort) is to construct tasks which require a model to ``chisel away'' the irrelevant information in the context, revealing a latent structure in the context. To verify a model's understanding of this latent structure, we query the model for details of the structure. Using \frameworkshort, we produce three diagnostic long-context evaluations across code and natural-language domains intended to provide a stronger signal of long-context language model capabilities. We perform evaluations on several state-of-the-art models and demonstrate both that a) the proposed evaluations are high-signal and b) that there is significant room for improvement in synthesizing long-context information.

난이도와 컨텍스트 길이가 쉽게 조절 가능하고 평가가 쉬우면서도 Needle in the Haystack보다 더 흥미로운(?) 벤치마크.

컨텍스트 길이가 길어지면 성능이 저하되는 이유는 무엇일까, 그리고 동시에 일정한 수준의 성능이 더 긴 컨텍스트 길이에 대해서도 유지되는 이유는 무엇일까에 대해서 잠깐 생각해보게 되네요. 무언가 짧은 길이와 긴 길이라는 두 그룹에 차이가 있고 긴 길이 내에서는 길이는 중요하지 않다는 의미 같기도 합니다.

#long-context #benchmark 