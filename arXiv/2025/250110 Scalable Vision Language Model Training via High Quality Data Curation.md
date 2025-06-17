https://arxiv.org/abs/2501.05952

*Scalable Vision Language Model Training via High Quality Data Curation* (Hongyuan Dong, Zijian Kang, Weijie Yin, Xiao Liang, Chao Feng, Jiao Ran)

> In this paper, we introduce SAIL-VL (ScAlable Vision Language Model TraIning via High QuaLity Data Curation), an open-source vision language model (VLM) of state-of-the-art (SOTA) performance with 2B parameters. We introduce three key improvements that contribute to SAIL-VL's leading performance: (1) Scalable high-quality visual understanding data construction: We implement a visual understanding data construction pipeline, which enables hundred-million-scale high-quality recaption data annotation. Equipped with this pipeline, we curate SAIL-Caption, a large-scale caption dataset with large quantity and the highest data quality compared with opensource caption datasets. (2) Scalable Pretraining with High-Quality Visual Understanding Data: We scale SAIL-VL's pretraining budget up to 131B tokens and show that even a 2B VLM benefits from scaled up training data sizes, exhibiting expected data size scaling laws in visual understanding and instruction following performance. (3) Scalable SFT via quantity and quality scaling: We introduce general guidance for instruction data curation to scale up instruction data continuously, allowing us to construct a large SFT dataset with the highest quality. To further improve SAIL-VL's performance, we propose quality scaling, a multi-stage training recipe with curriculum learning, to improve model performance scaling curves w.r.t. data sizes from logarithmic to be near-linear. SAIL-VL obtains the highest average score in 19 commonly used benchmarks in our evaluation and achieves top1 performance among VLMs of comparable sizes on OpenCompass (https://rank.opencompass.org.cn/leaderboard-multimodal). We release our SAIL-VL-2B model at HuggingFace (https://huggingface.co/BytedanceDouyinContent/SAIL-VL-2B).

Vision Language 프리트레이닝과 SFT의 규모 증대를 통한 성능 향상. 프리트레이닝은 Recaptioning을 통한 데이터 구축이 중심이고 SFT는 각 데이터소스에 대해서 소규모 실험으로 퀄리티를 평가해나가는 것이 중심이군요.

<english>
Improving performance of vision language models by scaling up pretraining and SFT. On pretraining main method is construction of data by recaptioning, and on SFT main point is evaluating quality of each data sources by doing small scale experiment.
</english>

#vision-language #captioning #scaling-law 