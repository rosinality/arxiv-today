https://arxiv.org/abs/2410.01692

*U-shaped and Inverted-U Scaling behind Emergent Abilities of Large Language Models* (Tung-Yu Wu, Pei-Yu Lo)

> Large language models (LLMs) have been shown to exhibit emergent abilities in some downstream tasks, where performance seems to stagnate at first and then improve sharply and unpredictably with scale beyond a threshold. By dividing questions in the datasets according to difficulty level by average performance, we observe U-shaped scaling for hard questions, and inverted-U scaling followed by steady improvement for easy questions. Moreover, the emergence threshold roughly coincides with the point at which performance on easy questions reverts from inverse scaling to standard scaling. Capitalizing on the observable though opposing scaling trend on easy and hard questions, we propose a simple yet effective pipeline, called Slice-and-Sandwich, to predict both the emergence threshold and model performance beyond the threshold.

LLM의 창발 현상에 대한 분석. 모델의 규모에 대해 문제의 난이도로 나눠 분석했군요. 흥미로운 점은 쉬운 문제들에 대해서는 Inverse-U 형태의 Scaling이 나타나고 어려운 문제들에 대해서는 U 형태의 Scaling이 나타난다고 합니다. 그리고 쉬운 문제들에 대해서 커브가 꺾이는 지점에서 창발이 일어난다고 하네요. 

Inverse U Scaling은 Double Descent와 비슷하고 U Scaling은 Inverse Scaling에서 모델 규모의 증가에 따라 Scaling 패턴으로 변화하는 형태죠. 상당히 흥미로운 설명이네요.

<english>
Analysis on emergent phenomena of LLMs. It analyzed performance of different model sizes grouped by difficulties of the problem. Interesting point is that for easy problems there are inverse U shaped scalingss. And for hard problems it shows U shaped scalings. And at the elbow point of the curve of easy problems emergence happens.

Inverse U scaling is similar to double descent, and U scaling is the pattern of from inverse scaling to normal scaling with increase of model scales. Very interesting explanation on emergent phenomena.
</english>

#scaling-law 