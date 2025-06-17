https://arxiv.org/abs/2403.17887

*The Unreasonable Ineffectiveness of the Deeper Layers* (Andrey Gromov, Kushal Tirumala, Hassan Shapourian, Paolo Glorioso, Daniel A. Roberts)

> We empirically study a simple layer-pruning strategy for popular families of open-weight pretrained LLMs, finding minimal degradation of performance on different question-answering benchmarks until after a large fraction (up to half) of the layers are removed. To prune these models, we identify the optimal block of layers to prune by considering similarity across layers; then, to "heal" the damage, we perform a small amount of finetuning. In particular, we use parameter-efficient finetuning (PEFT) methods, specifically quantization and Low Rank Adapters (QLoRA), such that each of our experiments can be performed on a single A100 GPU. From a practical perspective, these results suggest that layer pruning methods can complement other PEFT strategies to further reduce computational resources of finetuning on the one hand, and can improve the memory and latency of inference on the other hand. From a scientific perspective, the robustness of these LLMs to the deletion of layers implies either that current pretraining methods are not properly leveraging the parameters in the deeper layers of the network or that the shallow layers play a critical role in storing knowledge.

레이어의 입출력 유사도를 측정해서 유사도가 높은 레이어를 Pruning 하고 QLoRA로 레이어 Pruning의 영향을 감소시켜본 시도. 얼마 전에도 Self Attention을 타겟해서 Redundant한 레이어를 Pruing하고 Adapter를 사용해 Pruning의 효과를 상쇄하려는 시도가 나왔습니다. (https://arxiv.org/abs/2403.15226)

사실 레이어의 입출력이 비슷하다는 것은 Undertrain 됐다는 의미일 수도 있겠죠. (https://huggingface.co/blog/lorinma/yi-9b-divedeep) 따라서 학습이 더 진행된다면 Pruning이 어려워지는 효과도 있을 수 있지 않을까 싶긴 합니다만 일단 그래프에서는 Mistral에서도 그럭저럭 되는 것 같네요. Overtraining을 한다고 하더라도 Redundant한 레이어가 없어지지는 않을 것 같긴 합니다.

#pruning

# Links

