https://arxiv.org/abs/2411.12986

*Training Bilingual LMs with Data Constraints in the Targeted Language* (Skyler Seto, Maartje ter Hoeve, He Bai, Natalie Schluter, David Grangier)

> Large language models are trained on massive scrapes of the web, as required by current scaling laws. Most progress is made for English, given its abundance of high-quality pretraining data. For most other languages, however, such high quality pretraining data is unavailable. In this work, we study how to boost pretrained model performance in a data constrained target language by enlisting data from an auxiliary language for which high quality data is available. We study this by quantifying the performance gap between training with data in a data-rich auxiliary language compared with training in the target language, exploring the benefits of translation systems, studying the limitations of model scaling for data constrained languages, and proposing new methods for upsampling data from the auxiliary language. Our results show that stronger auxiliary datasets result in performance gains without modification to the model or training objective for close languages, and, in particular, that performance gains due to the development of more information-rich English pretraining datasets can extend to targeted language settings with limited data.

영어 데이터셋 같은 대량의 데이터셋을 확보할 수 있는 언어를 통한 데이터 양이 적은 언어에 대한 성능 개선 패턴 분석. 고품질의 영어 데이터셋을 활용하면 성능이 향상되는데 데이터셋을 걸러내는 것보다는 고가치의 정보가 포함되는 것이 중요하다는 것, 그리고 기계 번역 데이터 등이 도움이 된다는 결과네요. 다만 늘 그렇듯 언어마다 패턴이 다르다는 문제가 있긴 합니다.

<english>
Analysis on performance enhancement of low resource languages through abundant languages like english. We can enhance performances with more higher quality english datasets, and it comes from high quality informations rather than filtering, and machine translated texts can be beneficial. But as always, pattern is different among the languages.
</english>

#multilingual 