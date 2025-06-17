https://arxiv.org/abs/2309.16039

Effective Long-Context Scaling of Foundation Models (Wenhan Xiong, Jingyu Liu, Igor Molybog, Hejia Zhang, Prajjwal Bhargava, Rui Hou, Louis Martin, Rashi Rungta, Karthik Abinav Sankararaman, Barlas Oguz, Madian Khabsa, Han Fang, Yashar Mehdad, Sharan Narang, Kshitiz Malik, Angela Fan, Shruti Bhosale, Sergey Edunov, Mike Lewis, Sinong Wang, Hao Ma)

Llama-2의 context length 확장. Code Llama (https://arxiv.org/abs/2308.12950) 에서와 같이 rope의 base frequency를 증가시키고 파인튜닝하는 방법을 사용했습니다. rope + base frequency 증가 트릭이 꽤 잘 작동하는 것처럼 보이네요. 그 외에 짧은 길이로 프리트레이닝하고 긴 길이로 파인튜닝하는 커리큘럼이 효과적이라는 것을 다시 확인했습니다.

그러나 중요한 것은 파인튜닝한 데이터의 구성인데 여기에 대한 힌트는 거의 없네요. Llama 2의 프리트레이닝 데이터를 사용했을 때 짧은 길이의 데이터만으로 파인튜닝하거나 혹은 긴 길이의 데이터의 비율을 높인다거나 했을 때에도 (둘 다 파인튜닝 하지 않은 베이스라인보다 향상은 있었지만) 차이는 크게 없었고, 추가적인 긴 길이의 데이터 샘플이 들어갔을 때 효과가 있었다고 합니다. 그러니까 긴 길이의 샘플이 딱히 많을 필요는 없고 그 샘플의 퀄리티가 높아야 한다는 것을 시사하고 있습니다. 물론 그 높은 퀄리티의 샘플을 어떻게 구성한 것인지에 대해서는 그다지 말하고 있지 않습니다. 요즘 Weight도 공개하고 방법도 대략 공개하는 경우는 많지만 학습 데이터에 대해서는 거의 공개하지 않는 것이 흐름이군요.

#long_context

# Links

# Links

