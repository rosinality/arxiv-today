https://arxiv.org/abs/2309.12307

LongLoRA: Efficient Fine-tuning of Long-Context Large Language Models (Yukang Chen, Shengju Qian, Haotian Tang, Xin Lai, Zhijian Liu, Song Han, Jiaya Jia)

efficient long context finetuning. local attention을 사용하되 헤드 절반은 시퀀스를 shift해서 local window 사이에 overlap이 발생하게 합니다. 이 패턴을 사용했을 때 추론 시에는 그냥 full attention을 사용할 수 있었다고 하네요. lora를 사용하는데 lora만으로는 부족하기에 임베딩과 normalization 레이어를 같이 튜닝.

뭔가 LM-Infinite (https://arxiv.org/abs/2308.16137) 이 생각나기도 하네요. 다만 extrapolation이 아니라 그냥 long context finetuning을 하자는 쪽으로 무게중심이 쏠리는 것 같기도 합니다. 그리고 long context finetuning을 할 것이라면, 사실 자원이 있다면 full finetuning을 고려하는 것이 나을 수도 있겠죠.

#transformer #long_context

# Links

[[230830 LM-Infinite.md]]