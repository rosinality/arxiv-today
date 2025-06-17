https://arxiv.org/abs/2505.22018

*Improving Continual Pre-training Through Seamless Data Packing* (Ruicheng Yin, Xuan Gao, Changze Lv, Xiaohua Wang, Xiaoqing Zheng, Xuanjing Huang)

> Continual pre-training has demonstrated significant potential in enhancing model performance, particularly in domain-specific scenarios. The most common approach for packing data before continual pre-training involves concatenating input texts and splitting them into fixed-length sequences. While straightforward and efficient, this method often leads to excessive truncation and context discontinuity, which can hinder model performance. To address these issues, we explore the potential of data engineering to enhance continual pre-training, particularly its impact on model performance and efficiency. We propose Seamless Packing (SP), a novel data packing strategy aimed at preserving contextual information more effectively and enhancing model performance. Our approach employs a sliding window technique in the first stage that synchronizes overlapping tokens across consecutive sequences, ensuring better continuity and contextual coherence. In the second stage, we adopt a First-Fit-Decreasing algorithm to pack shorter texts into bins slightly larger than the target sequence length, thereby minimizing padding and truncation. Empirical evaluations across various model architectures and corpus domains demonstrate the effectiveness of our method, outperforming baseline method in 99% of all settings. Code is available at https://github.com/Infernus-WIND/Seamless-Packing.

Sequence Packing 연구. 문서 청크에 Sliding Window 형태로 추가 컨텍스트를 붙여주는 건 흥미롭네요.

<english>
Study on sequence packing. Adding additional context by using sliding window for document chunks is interesting.
</english>

#continual-learning 