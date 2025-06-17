https://arxiv.org/abs/2412.10117

*CosyVoice 2: Scalable Streaming Speech Synthesis with Large Language Models* (Zhihao Du, Yuxuan Wang, Qian Chen, Xian Shi, Xiang Lv, Tianyu Zhao, Zhifu Gao, Yexin Yang, Changfeng Gao, Hui Wang, Fan Yu, Huadai Liu, Zhengyan Sheng, Yue Gu, Chong Deng, Wen Wang, Shiliang Zhang, Zhijie Yan, Jingren Zhou)

> In our previous work, we introduced CosyVoice, a multilingual speech synthesis model based on supervised discrete speech tokens. By employing progressive semantic decoding with two popular generative models, language models (LMs) and Flow Matching, CosyVoice demonstrated high prosody naturalness, content consistency, and speaker similarity in speech in-context learning. Recently, significant progress has been made in multi-modal large language models (LLMs), where the response latency and real-time factor of speech synthesis play a crucial role in the interactive experience. Therefore, in this report, we present an improved streaming speech synthesis model, CosyVoice 2, which incorporates comprehensive and systematic optimizations. Specifically, we introduce finite-scalar quantization to improve the codebook utilization of speech tokens. For the text-speech LM, we streamline the model architecture to allow direct use of a pre-trained LLM as the backbone. In addition, we develop a chunk-aware causal flow matching model to support various synthesis scenarios, enabling both streaming and non-streaming synthesis within a single model. By training on a large-scale multilingual dataset, CosyVoice 2 achieves human-parity naturalness, minimal response latency, and virtually lossless synthesis quality in the streaming mode. We invite readers to listen to the demos at https://funaudiollm.github.io/cosyvoice2.

ASR 학습으로 추출한 FSQ 토큰을 시맨틱 토큰으로 사용해서 텍스트-음성에 대한 Autoregressive 학습을 하고, Mel Spectrogram은 레퍼런스 음성과 Flow Matching을 사용해 생성하는 방법. 논문에서 밝히고 있는 것처럼 텍스트 입력을 통해 생성되는 음성의 스타일을 지정할 수는 없는 구조네요.

실시간 출력이 되어야만 한다는 제약 조건이 모델링 선택을 흥미롭게 만드는 것 같습니다. 이미지 쪽에서도 Autoregressive 생성에 대한 진전이 많이 있는데, 결합해서 생각하면 재미있을 것 같네요.

<english>
Training the autoregressive model on semantic FSQ tokens which is extracted using ASR, and generates mel spectrogram using reference speech and flow matching. As the authors stated in the paper it is structure not allows modulate the style of speech using text inputs.

I think the restrictions that you should be able to generate outputs in real time maskes model choices interesting. Recently there was a lot progress on autoregressive image generation, and I think it would be interesting to combine the result of it with speech generation.
</english>

#autoregressive-model #text-to-speech #vq #flow-matching 