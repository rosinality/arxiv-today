https://arxiv.org/abs/2410.17251

*Altogether: Image Captioning via Re-aligning Alt-text* (Hu Xu, Po-Yao Huang, Xiaoqing Ellen Tan, Ching-Feng Yeh, Jacob Kahn, Christine Jou, Gargi Ghosh, Omer Levy, Luke Zettlemoyer, Wen-tau Yih, Shang-Wen Li, Saining Xie, Christoph Feichtenhofer)

> This paper focuses on creating synthetic data to improve the quality of image captions. Existing works typically have two shortcomings. First, they caption images from scratch, ignoring existing alt-text metadata, and second, lack transparency if the captioners' training data (e.g. GPT) is unknown. In this paper, we study a principled approach Altogether based on the key idea to edit and re-align existing alt-texts associated with the images. To generate training data, we perform human annotation where annotators start with the existing alt-text and re-align it to the image content in multiple rounds, consequently constructing captions with rich visual concepts. This differs from prior work that carries out human annotation as a one-time description task solely based on images and annotator knowledge. We train a captioner on this data that generalizes the process of re-aligning alt-texts at scale. Our results show our Altogether approach leads to richer image captions that also improve text-to-image generation and zero-shot image classification tasks.

Alt 텍스트를 기반으로 개선된 캡션을 만드는 작업을 반복해서 캡션을 작성하는 방법. 사람을 통해 직접 데이터를 구축했군요. 웹 데이터의 좋은 점은 그 무궁무진한 다양성이라고 생각하는데 단순한 캡셔닝은 이 다양성을 떨어뜨릴 가능성이 있겠죠. Alt 텍스트를 활용하는 것은 그 점에서 좋은 접근이리라고 생각합니다.

<english>
Generating captions by iterating refining captions, starting from alt texts. They employed human to write the data. What is nice thing about web data is huge diversity. And simple captioning can reduce
it. So I think it is good approach to use alt text in that aspect.
</english>

#captioning #dataset #image-text 