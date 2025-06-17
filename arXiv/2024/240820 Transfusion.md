https://arxiv.org/abs/2408.11039

*Transfusion: Predict the Next Token and Diffuse Images with One Multi-Modal Model* (Chunting Zhou, Lili Yu, Arun Babu, Kushal Tirumala, Michihiro Yasunaga, Leonid Shamis, Jacob Kahn, Xuezhe Ma, Luke Zettlemoyer, Omer Levy)

> We introduce Transfusion, a recipe for training a multi-modal model over discrete and continuous data. Transfusion combines the language modeling loss function (next token prediction) with diffusion to train a single transformer over mixed-modality sequences. We pretrain multiple Transfusion models up to 7B parameters from scratch on a mixture of text and image data, establishing scaling laws with respect to a variety of uni- and cross-modal benchmarks. Our experiments show that Transfusion scales significantly better than quantizing images and training a language model over discrete image tokens. By introducing modality-specific encoding and decoding layers, we can further improve the performance of Transfusion models, and even compress each image to just 16 patches. We further demonstrate that scaling our Transfusion recipe to 7B parameters and 2T multi-modal tokens produces a model that can generate images and text on a par with similar scale diffusion models and language models, reaping the benefits of both worlds.

텍스트는 Autoregression으로, 이미지는 Diffusion으로라는 아이디어의 연장선. (https://arxiv.org/abs/2403.05196, https://arxiv.org/abs/2406.11838) 여기서는 더 극단적으로 이미지에 대해서는 Causal Mask를 빼버렸고 입력 이미지 토큰 자체에 노이즈를 주입했습니다. 물론 이러면 Captioning에서는 문제가 될 수 있으니 배치 내 일부 샘플에는 최대 노이즈에 한도를 걸었네요.

저는 이런 결합이 인식과 생성을 동시에 잡을 수 있는 유망한 방법이 아닐까 싶습니다. 물론 더 심플한 방법이 가능하다면 좋겠지만요. (이것도 규모가 커지면 상관이 없어질 문제일지도 모르겠네요.)

#autoregressive-model #diffusion

# Links

[[240617 Autoregressive Image Generation without Vector Quantization.md]]
[[240308 Denoising Autoregressive Representation Learning.md]]