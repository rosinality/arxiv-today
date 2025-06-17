https://arxiv.org/abs/2411.03313

*Classification Done Right for Vision-Language Pre-Training* (Huang Zilong, Ye Qinghao, Kang Bingyi, Feng Jiashi, Fan Haoqi)

> We introduce SuperClass, a super simple classification method for vision-language pre-training on image-text data. Unlike its contrastive counterpart CLIP who contrast with a text encoder, SuperClass directly utilizes tokenized raw text as supervised classification labels, without the need for additional text filtering or selection. Due to the absence of the text encoding as contrastive target, SuperClass does not require a text encoder and does not need to maintain a large batch size as CLIP does. SuperClass demonstrated superior performance on various downstream tasks, including classic computer vision benchmarks and vision language downstream tasks. We further explored the scaling behavior of SuperClass on model size, training length, or data size, and reported encouraging results and comparisons to CLIP. https://github.com/x-cls/superclass

이미지 백본 프리트레이닝을 캡션의 단어들에 대한 Bag of Words 예측으로 진행하는 방법. 순서에 대한 고려를 빼고 Bag of Words로 Objective를 바꾸는 것은 종종 등장하긴 하죠.

<english>
Pretrain image backbones by predicting bag of words in the caption. It is often appears that ignoring ordering in the text and turning objective into bag of words prediction.
</english>

#clip 