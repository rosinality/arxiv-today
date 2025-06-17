https://arxiv.org/abs/2410.20796

*Rephrasing natural text data with different languages and quality levels for Large Language Model pre-training* (Michael Pieler, Marco Bellagente, Hannah Teufel, Duy Phung, Nathan Cooper, Jonathan Tow, Paulo Rocha, Reshinth Adithyan, Zaid Alyafeai, Nikhil Pinnaparaju, Maksym Zhuravinskyi, Carlos Riquelme)

> Recently published work on rephrasing natural text data for pre-training LLMs has shown promising results when combining the original dataset with the synthetically rephrased data. We build upon previous work by replicating existing results on C4 and extending them with our optimized rephrasing pipeline to the English, German, Italian, and Spanish Oscar subsets of CulturaX. Our pipeline leads to increased performance on standard evaluation benchmarks in both the mono- and multilingual setup. In addition, we provide a detailed study of our pipeline, investigating the choice of the base dataset and LLM for the rephrasing, as well as the relationship between the model size and the performance after pre-training. By exploring data with different perceived quality levels, we show that gains decrease with higher quality. Furthermore, we find the difference in performance between model families to be bigger than between different model sizes. This highlights the necessity for detailed tests before choosing an LLM to rephrase large amounts of data. Moreover, we investigate the effect of pre-training with synthetic data on supervised fine-tuning. Here, we find increasing but inconclusive results that highly depend on the used benchmark. These results (again) highlight the need for better benchmarking setups. In summary, we show that rephrasing multilingual and low-quality data is a very promising direction to extend LLM pre-training data.

프리트레이닝 코퍼스를 LLM으로 Paraphrasing 하는 것의 효과에 대한 분석. 원 데이터와 섞어주는 것이 좋다는 것과 저품질 데이터를 개선하는 것에 효과가 국한된다는 결론.

<english>
Analysis on effectiveness of paraphrasing pretraining corpus. Conclusion is it is better to mix with original dataset, and the effectiveness is restricted to improve low quality data.
</english>

#synthetic-data 