https://arxiv.org/abs/2310.05344

SteerLM: Attribute Conditioned SFT as an (User-Steerable) Alternative to RLHF (Yi Dong, Zhilin Wang, Makesh Narsimhan Sreedhar, Xianchao Wu, Oleksii Kuchaiev)

OASST의 attribute label을 사용해서 텍스트에 대한 attribute prediction 모델을 만들고, 이 모델로 데이터셋에 attribute label을 부여한 다음 attribute label에 condition 하는 방식으로 SFT, 이후 높은 퀄리티에 해당하는 attribute label을 condition으로 주고 샘플링한 다음 샘플에 다시 attribute prediction 모델로 attribute label을 부여, 그리고 새로 부여된 attribute label로 다시 SFT 하는 순서군요.

전반적으로 Reward Conditioning (https://arxiv.org/abs/2302.08582) 을 연상시키는 방법입니다. OASST과 HH-RLHF 데이터셋 구성으로 상당히 인상적인 결과가 나왔네요.

#alignment

# Links

[[230216 Pretraining Language Models with Human Preferences.md]]