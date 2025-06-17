https://arxiv.org/abs/2504.05419

*Reasoning Models Know When They're Right: Probing Hidden States for Self-Verification* (Anqi Zhang, Yulin Chen, Jane Pan, Chen Zhao, Aurojit Panda, Jinyang Li, He He)

> Reasoning models have achieved remarkable performance on tasks like math and logical reasoning thanks to their ability to search during reasoning. However, they still suffer from overthinking, often performing unnecessary reasoning steps even after reaching the correct answer. This raises the question: can models evaluate the correctness of their intermediate answers during reasoning? In this work, we study whether reasoning models encode information about answer correctness through probing the model's hidden states. The resulting probe can verify intermediate answers with high accuracy and produces highly calibrated scores. Additionally, we find models' hidden states encode correctness of future answers, enabling early prediction of the correctness before the intermediate answer is fully formulated. We then use the probe as a verifier to decide whether to exit reasoning at intermediate answers during inference, reducing the number of inference tokens by 24\% without compromising performance. These findings confirm that reasoning models do encode a notion of correctness yet fail to exploit it, revealing substantial untapped potential to enhance their efficiency.

Probing으로 각 추론 단계에서 추출한 중간 답변이 정답인지 아닌지를 예측할 수 있다는 결과. 이런 자기 검증 능력이 추론 RL 과정에서 학습된 것이겠죠.

<english>
The result says it is possible to predict whether intermediate answers extracted from each reasoning steps is correct by probing. These kind of self-verification ability would be trained during reasoning RL.
</english>

#reasoning 