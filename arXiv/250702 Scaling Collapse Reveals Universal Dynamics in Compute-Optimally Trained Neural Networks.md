https://arxiv.org/abs/2507.02119

*Scaling Collapse Reveals Universal Dynamics in Compute-Optimally Trained Neural Networks* (Shikai Qiu, Lechao Xiao, Andrew Gordon Wilson, Jeffrey Pennington, Atish Agarwala)

> What scaling limits govern neural network training dynamics when model size and training time grow in tandem? We show that despite the complex interactions between architecture, training algorithms, and data, compute-optimally trained models exhibit a remarkably precise universality. Specifically, loss curves from models of varying sizes collapse onto a single universal curve when training compute and loss are normalized to unity at the end of training. With learning rate decay, the collapse becomes so tight that differences in the normalized curves across models fall below the noise floor of individual loss curves across random seeds, a phenomenon we term supercollapse. We observe supercollapse across learning rate schedules, datasets, and architectures, including transformers trained on next-token prediction, and find it breaks down when hyperparameters are scaled suboptimally, providing a precise and practical indicator of good scaling. We explain these phenomena by connecting collapse to the power-law structure in typical neural scaling laws, and analyzing a simple yet surprisingly effective model of SGD noise dynamics that accurately predicts loss curves across various learning rate schedules and quantitatively explains the origin of supercollapse.

Compute Optimal한 모델의 학습 과정에서 최종 Loss로 Loss를 나눠주면 Loss의 커브의 개형이 모델 크기와는 관계 없이 거의 일치한다는 발견에 대한 분석.

<english>
An analysis on discovery of if we divide loss by final loss then regardless of model sizes overall form of loss curve is almost same, during compute optimal model training.
</english>

#scaling-law 