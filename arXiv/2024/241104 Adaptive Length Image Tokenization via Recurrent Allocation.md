https://arxiv.org/abs/2411.02393

*Adaptive Length Image Tokenization via Recurrent Allocation* (Shivam Duggal, Phillip Isola, Antonio Torralba, William T. Freeman)

> Current vision systems typically assign fixed-length representations to images, regardless of the information content. This contrasts with human intelligence - and even large language models - which allocate varying representational capacities based on entropy, context and familiarity. Inspired by this, we propose an approach to learn variable-length token representations for 2D images. Our encoder-decoder architecture recursively processes 2D image tokens, distilling them into 1D latent tokens over multiple iterations of recurrent rollouts. Each iteration refines the 2D tokens, updates the existing 1D latent tokens, and adaptively increases representational capacity by adding new tokens. This enables compression of images into a variable number of tokens, ranging from 32 to 256. We validate our tokenizer using reconstruction loss and FID metrics, demonstrating that token count aligns with image entropy, familiarity and downstream task requirements. Recurrent token processing with increasing representational capacity in each iteration shows signs of token specialization, revealing potential for object / part discovery.

가변 길이 이미지 Tokenization. VQ로 추출한 2D 코드와 추가 1D 코드를 인코더 입력으로 주고 새로운 코드를 출력하는 것을 반복하는 방식이군요.

<english>
Variable length image tokenization. Iteratively extracts new 1D codes from the encoder which given an input with 2D codes from VQ and additional 1D codes.
</english>

#vq 