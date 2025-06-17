https://arxiv.org/abs/2502.04223

*Éclair -- Extracting Content and Layout with Integrated Reading Order for Documents* (Ilia Karmanov, Amala Sanjay Deshmukh, Lukas Voegtle, Philipp Fischer, Kateryna Chumachenko, Timo Roman, Jarno Seppänen, Jupinder Parmar, Joseph Jennings, Andrew Tao, Karan Sapra)

> Optical Character Recognition (OCR) technology is widely used to extract text from images of documents, facilitating efficient digitization and data retrieval. However, merely extracting text is insufficient when dealing with complex documents. Fully comprehending such documents requires an understanding of their structure -- including formatting, formulas, tables, and the reading order of multiple blocks and columns across multiple pages -- as well as semantic information for detecting elements like footnotes and image captions. This comprehensive understanding is crucial for downstream tasks such as retrieval, document question answering, and data curation for training Large Language Models (LLMs) and Vision Language Models (VLMs). To address this, we introduce \'Eclair, a general-purpose text-extraction tool specifically designed to process a wide range of document types. Given an image, \'Eclair is able to extract formatted text in reading order, along with bounding boxes and their corresponding semantic classes. To thoroughly evaluate these novel capabilities, we introduce our diverse human-annotated benchmark for document-level OCR and semantic classification. \'Eclair achieves state-of-the-art accuracy on this benchmark, outperforming other methods across key metrics. Additionally, we evaluate \'Eclair on established benchmarks, demonstrating its versatility and strength across several evaluation standards.

레이아웃 정보를 보존하는 OCR 모델. 논문에서도 언급하고 있지만 LLM 프리트레이닝을 위해선 이제 좋은 OCR 파이프라인을 갖고 있는 것도 중요한 문제가 아닐까 싶습니다.

<english>
OCR model that preserves layout information. As mentioned in the paper, it would be important to have a good OCR pipelines for LLM pretraining.
</english>

#ocr