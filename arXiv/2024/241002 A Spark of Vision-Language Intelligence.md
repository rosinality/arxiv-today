https://arxiv.org/abs/2410.01912

*A Spark of Vision-Language Intelligence: 2-Dimensional Autoregressive Transformer for Efficient Finegrained Image Generation* (Liang Chen, Sinan Tan, Zefan Cai, Weichu Xie, Haozhe Zhao, Yichi Zhang, Junyang Lin, Jinze Bai, Tianyu Liu, Baobao Chang)

> This work tackles the information loss bottleneck of vector-quantization (VQ) autoregressive image generation by introducing a novel model architecture called the 2-Dimensional Autoregression (DnD) Transformer. The DnD-Transformer predicts more codes for an image by introducing a new autoregression direction, \textit{model depth}, along with the sequence length direction. Compared to traditional 1D autoregression and previous work utilizing similar 2D image decomposition such as RQ-Transformer, the DnD-Transformer is an end-to-end model that can generate higher quality images with the same backbone model size and sequence length, opening a new optimization perspective for autoregressive image generation. Furthermore, our experiments reveal that the DnD-Transformer's potential extends beyond generating natural images. It can even generate images with rich text and graphical elements in a self-supervised manner, demonstrating an understanding of these combined modalities. This has not been previously demonstrated for popular vision generative models such as diffusion models, showing a spark of vision-language intelligence when trained solely on images. Code, datasets and models are open at https://github.com/chenllliang/DnD-Transformer.

요새 RQ-VAE로 (https://arxiv.org/abs/2203.01941) VQ의 제약을 해소하려는 연구들이 많이 나오는군요. 16x 다운샘플링, 16K Vocab, 8개의 코드를 사용하니 텍스트 이미지에 대해서도 거의 완벽하게 Reconstruction이 되는군요. OCR을 고려했다는 것이 마음에 드네요.

8개 코드를 생성하는 것이 문제인데 되도록 한 스텝 내에서 해결이 가능하도록 레이
어를 나눠 하나씩 생성해나가도록 설정했습니다. 이쪽도 꽤 흥미로운 디자인이네요.

<english>
Recently many researches emerging that tries to relieve limitations of VQ with RQ-VAE (https://arxiv.org/abs/2203.01941). With 16x downsampling, 16K Vocab, and 8 codes, it is possible to achieve almost perfect reconstruction even for text images. I like this paper considered for OCR.

Main problem is how can generate 8 tokens efficiently. In this work authors have let model to sample each tokens per layer blocks to allow model to sample entire codes within single step. I think this is quite interesting design.
</english>

#vq #autoregressive-model #image-generation

# Links

