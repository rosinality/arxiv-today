https://arxiv.org/abs/2401.18058

*LongAlign: A Recipe for Long Context Alignment of Large Language Models* (Yushi Bai, Xin Lv, Jiajie Zhang, Yuze He, Ji Qi, Lei Hou, Jie Tang, Yuxiao Dong, Juanzi Li)

> Extending large language models to effectively handle long contexts requires instruction fine-tuning on input sequences of similar length. To address this, we present LongAlign -- a recipe of the instruction data, training, and evaluation for long context alignment. First, we construct a long instruction-following dataset using Self-Instruct. To ensure the data diversity, it covers a broad range of tasks from various long context sources. Second, we adopt the packing and sorted batching strategies to speed up supervised fine-tuning on data with varied length distributions. Additionally, we develop a loss weighting method to balance the contribution to the loss across different sequences during packing training. Third, we introduce the LongBench-Chat benchmark for evaluating instruction-following capabilities on queries of 10k-100k in length. Experiments show that LongAlign outperforms existing recipes for LLMs in long context tasks by up to 30\%, while also maintaining their proficiency in handling short, generic tasks. The code, data, and long-aligned models are open-sourced at https://github.com/THUDM/LongAlign.

긴 Instruction 데이터에 대한 Instruction Tuning 실험 결과. 긴 Context를 요구하는 과제에는 긴 Instruction 데이터를 사용하는 것이 짧은 Context 과제들에 대한 성능 손실 없이 도움이 되고, 비슷한 길이끼리 묶어서 배치 혹은 패킹 + 길이에 따른 가중치 적용이 괜찮은 방법인 것 같다는 결과네요.

#instruction-tuning #long-context 

Experimental results on instruction tuning with long context instructions. Using long context data is beneficial for long context tasks, without compromising short sequence tasks. Making batches with similar lengths or using sequence packing with loss reweighting by length would be useful method for training with long samples.