https://arxiv.org/abs/2506.14761

*From Bytes to Ideas: Language Modeling with Autoregressive U-Nets* (Mathurin Videau, Badr Youbi Idrissi, Alessandro Leite, Marc Schoenauer, Olivier Teytaud, David Lopez-Paz)

> Tokenization imposes a fixed granularity on the input text, freezing how a language model operates on data and how far in the future it predicts. Byte Pair Encoding (BPE) and similar schemes split text once, build a static vocabulary, and leave the model stuck with that choice. We relax this rigidity by introducing an autoregressive U-Net that learns to embed its own tokens as it trains. The network reads raw bytes, pools them into words, then pairs of words, then up to 4 words, giving it a multi-scale view of the sequence. At deeper stages, the model must predict further into the future -- anticipating the next few words rather than the next byte -- so deeper stages focus on broader semantic patterns while earlier stages handle fine details. When carefully tuning and controlling pretraining compute, shallow hierarchies tie strong BPE baselines, and deeper hierarchies have a promising trend. Because tokenization now lives inside the model, the same system can handle character-level tasks and carry knowledge across low-resource languages.

바이트 UNet 형태의 시퀀스 모델인데 풀링에서 시퀀스를 쪼개는 메커니즘을 요구하는군요. 여기서는 공백으로 쪼개고 있습니다.

<english>
Byte UNet style sequence models, but it requires a mechanism for splitting sequences for poolings. This study used space based splitter.
</english>

#transformer #llm 