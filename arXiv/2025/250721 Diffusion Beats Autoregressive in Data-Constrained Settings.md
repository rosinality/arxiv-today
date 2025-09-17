https://arxiv.org/abs/2507.15857

*Diffusion Beats Autoregressive in Data-Constrained Settings* (Mihir Prabhudesai, Menging Wu, Amir Zadeh, Katerina Fragkiadaki, Deepak Pathak)

> Autoregressive (AR) models have long dominated the landscape of large language models, driving progress across a wide range of tasks. Recently, diffusion-based language models have emerged as a promising alternative, though their advantages over AR models remain underexplored. In this paper, we systematically study masked diffusion models in data-constrained settings-where training involves repeated passes over limited data-and find that they significantly outperform AR models when compute is abundant but data is scarce. Diffusion models make better use of repeated data, achieving lower validation loss and superior downstream performance. We interpret this advantage as implicit data augmentation: masked diffusion exposes the model to a diverse distribution of token orderings and prediction tasks, unlike AR's fixed left-to-right factorization. We find new scaling laws for diffusion models and derive a closed-form expression for the critical compute threshold at which diffusion begins to outperform AR. These results suggest that when data, not compute, is the bottleneck, diffusion models offer a compelling alternative to the standard AR paradigm. Our code is available at: https://diffusion-scaling.github.io.

최근 생각해보던 문제에 대한 연구가 나왔다. Diffusion은 더 다양한 입력에 모델을 노출시키기 때문에 Autoregressive 모델보다 Multi Epoch 사용에 더 강하지 않을까 하는 아이디어. 예측에 따르면 Trillion 단위의 토큰이 있다면 실용적으로는 상관 없는 문제이긴 하다.

A problem I've been thinking about recently. Diffusion might be more robust to multi-epoch than autoregressive models as it exposes the model to more diverse inputs. Though according to the predictions this wouldn't be a practical concern if you have trillions of tokens.

#scaling-law #diffusion #autoregressive-model 