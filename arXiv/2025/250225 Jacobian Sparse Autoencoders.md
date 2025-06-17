https://arxiv.org/abs/2502.18147

*Jacobian Sparse Autoencoders: Sparsify Computations, Not Just Activations* (Lucy Farnik, Tim Lawson, Conor Houghton, Laurence Aitchison)

> Sparse autoencoders (SAEs) have been successfully used to discover sparse and human-interpretable representations of the latent activations of LLMs. However, we would ultimately like to understand the computations performed by LLMs and not just their representations. The extent to which SAEs can help us understand computations is unclear because they are not designed to "sparsify" computations in any sense, only latent activations. To solve this, we propose Jacobian SAEs (JSAEs), which yield not only sparsity in the input and output activations of a given model component but also sparsity in the computation (formally, the Jacobian) connecting them. With a na\"ive implementation, the Jacobians in LLMs would be computationally intractable due to their size. One key technical contribution is thus finding an efficient way of computing Jacobians in this setup. We find that JSAEs extract a relatively large degree of computational sparsity while preserving downstream LLM performance approximately as well as traditional SAEs. We also show that Jacobians are a reasonable proxy for computational sparsity because MLPs are approximately linear when rewritten in the JSAE basis. Lastly, we show that JSAEs achieve a greater degree of computational sparsity on pre-trained LLMs than on the equivalent randomized LLM. This shows that the sparsity of the computational graph appears to be a property that LLMs learn through training, and suggests that JSAEs might be more suitable for understanding learned transformer computations than standard SAEs.

Sparse Autoencoder로 Latent를 분해하는 것을 넘어 모듈 내에서 일어나는 연산을 분해하겠다는 아이디어. 입력과 출력에 대해 SAE를 학습하면서 SAE Latent 사이의 Jacobian을 Sparse하게 만드는 방식으로 접근했네요.

<english>
Beyond decomposing latent they tried to decompose computation occuring inside the module using sparse autoencoder. They trained SAE at the input and output of the module and let jacobian to be spase between SAE latents.
</english>

#mechanistic-interpretation 