https://arxiv.org/abs/2411.04330

*Scaling Laws for Precision* (Tanishq Kumar, Zachary Ankner, Benjamin F. Spector, Blake Bordelon, Niklas Muennighoff, Mansheej Paul, Cengiz Pehlevan, Christopher Ré, Aditi Raghunathan)

> Low precision training and inference affect both the quality and cost of language models, but current scaling laws do not account for this. In this work, we devise "precision-aware" scaling laws for both training and inference. We propose that training in lower precision reduces the model's "effective parameter count," allowing us to predict the additional loss incurred from training in low precision and post-train quantization. For inference, we find that the degradation introduced by post-training quantization increases as models are trained on more data, eventually making additional pretraining data actively harmful. For training, our scaling laws allow us to predict the loss of a model with different parts in different precisions, and suggest that training larger models in lower precision may be compute optimal. We unify the scaling laws for post and pretraining quantization to arrive at a single functional form that predicts degradation from training and inference in varied precisions. We fit on over 465 pretraining runs and validate our predictions on model sizes up to 1.7B parameters trained on up to 26B tokens.

Quantized Training과 PTQ에 대한 Scaling Law. 흥미로운 점이 많습니다.

1. PTQ의 경우 프리트레이닝을 오버트레이닝을 할수록 정밀로 감소에 따른 Loss 증가가 커진다.
2. Quantized Training의 경우 모델 크기, 데이터, 정밀도를 모두 조정해서 연산 최적인 지점을 찾는다면 더 낮은 정밀도를 사용할 수 있다. 그러나 FP4 이하는 손실이 커진다.
3. 모델 크기를 고정하고 데이터 크기를 증가시킨다면 정밀도도 증가시키는 것이 최적일 수 있다.

<english>
Scaling law for quantized training and post training quantization. There are a lot of interesting points.

1. For PTQ, if we overtrain more in pretraining, loss difference due to decrease in precision increases.
2. For quantized training if we optimize all of model sizes, data, precision, and try to find compute optimal points, then we can use lower precision. But from FP4 loss is increasing.
3. If we fix the model size and increase the data then we also may need to increase the precision.
</english>

#quantization #scaling-law 