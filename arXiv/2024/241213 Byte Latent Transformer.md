https://dl.fbaipublicfiles.com/blt/BLT__Patches_Scale_Better_Than_Tokens.pdf

*Byte Latent Transformer: Patches Scale Better Than Tokens* (Artidoro Pagnoni, Ram Pasunuru, Pedro Rodriguez, John Nguyen, Benjamin Muller, Margaret Li, Chunting Zhou, Lili Yu, Jason Weston, Luke Zettlemoyer, Gargi Ghosh, Mike Lewis, Ari Holtzman, Srinivasan Iyer)

> We introduce the Byte Latent Transformer (BLT), a new byte-level LLM architecture that, for the first time, matches tokenization-based LLM performance at scale with significant improvements in inference efficiency and robustness. BLT encodes bytes into dynamically sized patches, which serve as the primary units of computation. Patches are segmented based on the entropy of the next byte, allocating more compute and model capacity where increased data complexity demands it. We present the first flop controlled scaling study of byte-level models up to 8B parameters and 4T training bytes. Our results demonstrate the feasibility of scaling models trained on raw bytes without a fixed vocabulary. Both training and inference efficiency improve due to dynamically selecting long patches when data is predictable, along with qualitative improvements on reasoning and long tail generalization. Overall, for fixed inference costs, BLT shows significantly better scaling than tokenization-based models, by simultaneously growing both patch and model size.

바이트 단위 LM. 바이트를 묶기 위해 작은 바이트 단위 LM으로 엔트로피를 측정해 엔트로피가 큰 지점에서 자르는 방식을 사용했습니다. BPE와는 달리 고정된 Vocabulary 없이 상황에 따라, 예측 난이도에 따라 다른 바이트 패치가 만들어질 수 있죠. 재미있네요.

<english>
Byte-level LM. To group bytes measure entropy using small byte-level LM and split bytes where entropy is large. Unlike BPE bytes can be grouped into patches considering contexts and prediction difficulties without fixed vocabulary. Interesting
</english>

#tokenizer 