https://arxiv.org/abs/2410.07524

*Upcycling Large Language Models into Mixture of Experts* (Ethan He, Abhinav Khattar, Ryan Prenger, Vijay Korthikanti, Zijie Yan, Tong Liu, Shiqing Fan, Ashwath Aithal, Mohammad Shoeybi, Bryan Catanzaro)

> Upcycling pre-trained dense language models into sparse mixture-of-experts (MoE) models is an efficient approach to increase the model capacity of already trained models. However, optimal techniques for upcycling at scale remain unclear. In this work, we conduct an extensive study of upcycling methods and hyperparameters for billion-parameter scale language models. We propose a novel "virtual group" initialization scheme and weight scaling approach to enable upcycling into fine-grained MoE architectures. Through ablations, we find that upcycling outperforms continued dense model training. In addition, we show that softmax-then-topK expert routing improves over topK-then-softmax approach and higher granularity MoEs can help improve accuracy. Finally, we upcycled Nemotron-4 15B on 1T tokens and compared it to a continuously trained version of the same model on the same 1T tokens: the continuous trained model achieved 65.3% MMLU, whereas the upcycled model achieved 67.6%. Our results offer insights and best practices to effectively leverage upcycling for building MoE language models.

Sparse Upcycling의 레시피 연구. LR이나 배치 크기를 어떻게 설정할 것인가, FFN을 쪼개 작은 Expert들로 나누는 방법 등을 탐색했습니다. 흥미로운 점은 FFN을 쪼개서 Dense 모델과 FLOP을 같게 만든 다음 Continual Pretraining을 했을 때 Dense 모델보다 더 나은 성능을 얻을 수 있다는 결과일 듯 하네요.

<english>
Study on recipe for sparse upcycling. How should we choose LR or batch sizes, or exploration of the method of split FFN into small experts. One interesting result is that splitting FFN to match flop with dense models, then do continual pretraining, then it was possible to get better result than dense models
</english>

#moe #continual-pretraining 