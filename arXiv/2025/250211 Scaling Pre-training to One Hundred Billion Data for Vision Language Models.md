https://arxiv.org/abs/2502.07617

*Scaling Pre-training to One Hundred Billion Data for Vision Language Models* (Xiao Wang, Ibrahim Alabdulmohsin, Daniel Salz, Zhe Li, Keran Rong, Xiaohua Zhai)

> We provide an empirical investigation of the potential of pre-training vision-language models on an unprecedented scale: 100 billion examples. We find that model performance tends to saturate at this scale on many common Western-centric classification and retrieval benchmarks, such as COCO Captions. Nevertheless, tasks of cultural diversity achieve more substantial gains from the 100-billion scale web data, thanks to its coverage of long-tail concepts. Furthermore, we analyze the model's multilinguality and show gains in low-resource languages as well. In addition, we observe that reducing the size of the pretraining dataset via quality filters like using CLIP, typically used to enhance performance, may inadvertently reduce the cultural diversity represented even in large-scale datasets. Our results highlight that while traditional benchmarks may not benefit significantly from scaling noisy, raw web data to 100 billion examples, this data scale is vital for building truly inclusive multimodal systems.

100B 규모의 SigLIP 학습. 대부분의 벤치마크는 10B 정도에서 포화되지만 문화적 Diversity를 포착하는 벤치마크에서는 향상이 있고, 퀄리티 필터링을 적용하면 이 Diversity 부분에서 편향이 발생하네요.

<english>
Training SigLIP in scale of 100B. Most benchmarks are saturated at 10B, but there are improvements in benchmarks catches cultural diversity, and quality filtering causes bias in this aspect of diversity.
</english>

#clip #pretraining 