https://arxiv.org/abs/2405.02793

*ImageInWords: Unlocking Hyper-Detailed Image Descriptions* (Roopal Garg, Andrea Burns, Burcu Karagol Ayan, Yonatan Bitton, Ceslee Montgomery, Yasumasa Onoe, Andrew Bunner, Ranjay Krishna, Jason Baldridge, Radu Soricut)

> Despite the longstanding adage "an image is worth a thousand words," creating accurate and hyper-detailed image descriptions for training Vision-Language models remains challenging. Current datasets typically have web-scraped descriptions that are short, low-granularity, and often contain details unrelated to the visual content. As a result, models trained on such data generate descriptions replete with missing information, visual inconsistencies, and hallucinations. To address these issues, we introduce ImageInWords (IIW), a carefully designed human-in-the-loop annotation framework for curating hyper-detailed image descriptions and a new dataset resulting from this process. We validate the framework through evaluations focused on the quality of the dataset and its utility for fine-tuning with considerations for readability, comprehensiveness, specificity, hallucinations, and human-likeness. Our dataset significantly improves across these dimensions compared to recently released datasets (+66%) and GPT-4V outputs (+48%). Furthermore, models fine-tuned with IIW data excel by +31% against prior work along the same human evaluation dimensions. Given our fine-tuned models, we also evaluate text-to-image generation and vision-language reasoning. Our model's descriptions can generate images closest to the original, as judged by both automated and human metrics. We also find our model produces more compositionally rich descriptions, outperforming the best baseline by up to 6% on ARO, SVO-Probes, and Winoground datasets.

고밀도 이미지 캡션 데이터셋 구축. 기본적으로 VLM이 생성한 출력을 사람이 개선하고, 개선된 데이터를 다시 사람이 평가하고 개선하면 이 데이터를 사용해 VLM을 파인튜닝하는 루프를 사용합니다.

첫 단계 과제로 Object Detection으로 객체들의 목록을 만든 다음 개선하고, 그리고 찾아낸 객체들과 캡션을 기반으로 상세한 캡션을 작성하는 과제를 수행합니다.

이렇게 9K 분량의 데이터셋을 구축했네요. 이미지 캡션 데이터셋의 끝을 보겠다는 느낌이군요.

#vision-language #captioning #dataset 