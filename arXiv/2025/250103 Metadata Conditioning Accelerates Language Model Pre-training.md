https://arxiv.org/abs/2501.01956

*Metadata Conditioning Accelerates Language Model Pre-training* (Tianyu Gao, Alexander Wettig, Luxi He, Yihe Dong, Sadhika Malladi, Danqi Chen)

> The vast diversity of styles, domains, and quality levels present in language model pre-training corpora is essential in developing general model capabilities, but efficiently learning and deploying the correct behaviors exemplified in each of these heterogeneous data sources is challenging. To address this, we propose a new method, termed Metadata Conditioning then Cooldown (MeCo), to incorporate additional learning cues during pre-training. MeCo first provides metadata (e.g., URLs like en.wikipedia.org) alongside the text during training and later uses a cooldown phase with only the standard text, thereby enabling the model to function normally even without metadata. MeCo significantly accelerates pre-training across different model scales (600M to 8B parameters) and training sources (C4, RefinedWeb, and DCLM). For instance, a 1.6B language model trained with MeCo matches the downstream task performance of standard pre-training while using 33% less data. Additionally, MeCo enables us to steer language models by conditioning the inference prompt on either real or fabricated metadata that encodes the desired properties of the output: for example, prepending wikipedia.org to reduce harmful generations or factquizmaster.com (fabricated) to improve common knowledge task performance. We also demonstrate that MeCo is compatible with different types of metadata, such as model-generated topics. MeCo is remarkably simple, adds no computational overhead, and demonstrates promise in producing more capable and steerable language models.

프리트레이닝 문서 앞에 문서 URL을 붙이는 방법으로 학습 속도 가속. 물론 문서 URL이 주어지지 않으면 성능이 깎이기에 학습 후반에는 URL 없이 학습을 시킵니다.

<english>
Accelerating pre-training speed by appending URL to the documents. Of course performances will be reduced if URL is not given, so they trained model without URL during late stage of training.
</english>

#pre-training 