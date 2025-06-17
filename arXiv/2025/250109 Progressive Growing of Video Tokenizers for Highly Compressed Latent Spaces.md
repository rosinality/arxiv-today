https://arxiv.org/abs/2501.05442

*Progressive Growing of Video Tokenizers for Highly Compressed Latent Spaces* (Aniruddha Mahapatra, Long Mai, Yitian Zhang, David Bourgin, Feng Liu)

> Video tokenizers are essential for latent video diffusion models, converting raw video data into spatiotemporally compressed latent spaces for efficient training. However, extending state-of-the-art video tokenizers to achieve a temporal compression ratio beyond 4x without increasing channel capacity poses significant challenges. In this work, we propose an alternative approach to enhance temporal compression. We find that the reconstruction quality of temporally subsampled videos from a low-compression encoder surpasses that of high-compression encoders applied to original videos. This indicates that high-compression models can leverage representations from lower-compression models. Building on this insight, we develop a bootstrapped high-temporal-compression model that progressively trains high-compression blocks atop well-trained lower-compression models. Our method includes a cross-level feature-mixing module to retain information from the pretrained low-compression model and guide higher-compression blocks to capture the remaining details from the full video sequence. Evaluation of video benchmarks shows that our method significantly improves reconstruction quality while increasing temporal compression compared to direct extensions of existing video tokenizers. Furthermore, the resulting compact latent space effectively trains a video diffusion model for high-quality video generation with a reduced token budget.

비디오 토크나이저의 시간축의 압축률을 높이기 위한 방법. 16x 압축은 그냥은 안 되지만 4x 압축 모델로 4x 서브샘플링한 프레임을 압축하는 것은 된다는 것에서 시작했네요. 그러니까 시간축이 증가하면서 움직임의 양이 늘어나는 것 자체는 문제가 아닐 수 있다는 것입니다. 그래서 서브샘플링한 비디오를 인코딩한 결과를 추가 입력으로 사용해 가이드를 주는 방법을 생각했군요.

<english>
A method for increasing compression rate along temporal axis of video tokenizer. It starts from 16x compression from scratch is not feasible, but it is possible to compress 4x subsampled frame with 4x compression models. That suggests, increasement of the amount of motion with increasing temporal axis itself is maybe not problematic. So they thought give a guidance by using encoded features of subsampled video as an additional input.
</english>

#video #tokenizer 