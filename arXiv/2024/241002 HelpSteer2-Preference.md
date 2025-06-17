https://arxiv.org/abs/2410.01257

*HelpSteer2-Preference: Complementing Ratings with Preferences* (Zhilin Wang, Alexander Bukharin, Olivier Delalleau, Daniel Egert, Gerald Shen, Jiaqi Zeng, Oleksii Kuchaiev, Yi Dong)

> Reward models are critical for aligning models to follow instructions, and are typically trained following one of two popular paradigms: Bradley-Terry style or Regression style. However, there is a lack of evidence that either approach is better than the other, when adequately matched for data. This is primarily because these approaches require data collected in different (but incompatible) formats, meaning that adequately matched data is not available in existing public datasets. To tackle this problem, we release preference annotations (designed for Bradley-Terry training) to complement existing ratings (designed for Regression style training) in the HelpSteer2 dataset. To improve data interpretability, preference annotations are accompanied with human-written justifications. Using this data, we conduct the first head-to-head comparison of Bradley-Terry and Regression models when adequately matched for data. Based on insights derived from such a comparison, we propose a novel approach to combine Bradley-Terry and Regression reward modeling. A Llama-3.1-70B-Instruct model tuned with this approach scores 94.1 on RewardBench, emerging top of more than 140 reward models as of 1 Oct 2024. We also demonstrate the effectiveness of this reward model at aligning models to follow instructions in RLHF. We open-source this dataset (CC-BY-4.0 license) at https://huggingface.co/datasets/nvidia/HelpSteer2 and openly release the trained Reward Model at https://huggingface.co/nvidia/Llama-3.1-Nemotron-70B-Reward

HelpSteer2에서 (https://arxiv.org/abs/2406.08673) 했던 Likert Scale 어노테이션에 대해 Pairwise Preference 스타일 어노테이션을 진행해 Reward Model을 Regression으로 학습한 것과 Bradley-Terry 모델로 학습한 것을 비교해봤네요.

<english>
In addition to Liker scale annotation in HelpSteer2 (https://arxiv.org/abs/2406.08673) They did pairwise prefence style annotation, and compared reward models trained with regression or Bradley-Terry.
</english>

#reward-model

# Links

[[240612 HelpSteer2.md]]