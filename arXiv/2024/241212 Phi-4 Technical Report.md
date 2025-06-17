https://arxiv.org/abs/2412.08905

*Phi-4 Technical Report* (Marah Abdin, Jyoti Aneja, Harkirat Behl, Sébastien Bubeck, Ronen Eldan, Suriya Gunasekar, Michael Harrison, Russell J. Hewett, Mojan Javaheripi, Piero Kauffmann, James R. Lee, Yin Tat Lee, Yuanzhi Li, Weishung Liu, Caio C. T. Mendes, Anh Nguyen, Eric Price, Gustavo de Rosa, Olli Saarikivi, Adil Salim, Shital Shah, Xin Wang, Rachel Ward, Yue Wu, Dingli Yu, Cyril Zhang, Yi Zhang)

> We present phi-4, a 14-billion parameter language model developed with a training recipe that is centrally focused on data quality. Unlike most language models, where pre-training is based primarily on organic data sources such as web content or code, phi-4 strategically incorporates synthetic data throughout the training process. While previous models in the Phi family largely distill the capabilities of a teacher model (specifically GPT-4), phi-4 substantially surpasses its teacher model on STEM-focused QA capabilities, giving evidence that our data-generation and post-training techniques go beyond distillation. Despite minimal changes to the phi-3 architecture, phi-4 achieves strong performance relative to its size -- especially on reasoning-focused benchmarks -- due to improved data, training curriculum, and innovations in the post-training scheme.

Phi-4가 나왔군요. Phi 스타일의 합성 데이터가 벤치마크 스코어를 굉장히 높게 끌어올린다는 것은 분명하겠죠. 이것이 실제 유용성과 연결이 된다면 괜찮겠지만 그렇지 않다면 벤치마크 성능이 판단의 기준이 되기 어렵다는 의미일 겁니다. 합성 데이터가 중요한 역할을 할 수 있으리라고 생각하지만 만약 벤치마크 스코어가 충분한 지표가 되지 않는다면 판단에 보다 조심스러워져야만 하겠죠.

<english>
Phi-4 is came out. It is apparent that Phi style synthetic data can vastly improve benchmark scores. If this relates well actual usefulness then it would be nice, but if not, then it will mean that benchmark scores cannot be a criteria for making decisions about the data. I think synthetic data can do a significant role but if benchmark scores cannot be sufficient metrics then we should be more cautious about these kind of decisions.
</english>

#llm #synthetic-data 