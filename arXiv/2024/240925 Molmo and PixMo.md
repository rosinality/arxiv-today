https://arxiv.org/abs/2409.17146

*Molmo and PixMo: Open Weights and Open Data for State-of-the-Art Multimodal Models* (Matt Deitke, Christopher Clark, Sangho Lee, Rohun Tripathi, Yue Yang, Jae Sung Park, Mohammadreza Salehi, Niklas Muennighoff, Kyle Lo, Luca Soldaini, Jiasen Lu, Taira Anderson, Erin Bransom, Kiana Ehsani, Huong Ngo, YenSung Chen, Ajay Patel, Mark Yatskar, Chris Callison-Burch, Andrew Head, Rose Hendrix, Favyen Bastani, Eli VanderBilt, Nathan Lambert, Yvonne Chou, Arnavi Chheda, Jenna Sparks, Sam Skjonsberg, Michael Schmitz, Aaron Sarnat, Byron Bischoff, Pete Walsh, Chris Newell, Piper Wolters, Tanmay Gupta, Kuo-Hao Zeng, Jon Borchardt, Dirk Groeneveld, Jen Dumas, Crystal Nam, Sophie Lebrecht, Caitlin Wittlif, Carissa Schoenick, Oscar Michel, Ranjay Krishna, Luca Weihs, Noah A. Smith, Hannaneh Hajishirzi, Ross Girshick, Ali Farhadi, Aniruddha Kembhavi)

> Today's most advanced multimodal models remain proprietary. The strongest open-weight models rely heavily on synthetic data from proprietary VLMs to achieve good performance, effectively distilling these closed models into open ones. As a result, the community is still missing foundational knowledge about how to build performant VLMs from scratch. We present Molmo, a new family of VLMs that are state-of-the-art in their class of openness. Our key innovation is a novel, highly detailed image caption dataset collected entirely from human annotators using speech-based descriptions. To enable a wide array of user interactions, we also introduce a diverse dataset mixture for fine-tuning that includes in-the-wild Q&A and innovative 2D pointing data. The success of our approach relies on careful choices for the model architecture details, a well-tuned training pipeline, and, most critically, the quality of our newly collected datasets, all of which will be released. The best-in-class 72B model within the Molmo family not only outperforms others in the class of open weight and data models but also compares favorably against proprietary systems like GPT-4o, Claude 3.5, and Gemini 1.5 on both academic benchmarks and human evaluation. We will be releasing all of our model weights, captioning and fine-tuning data, and source code in the near future. Select model weights, inference code, and demo are available at https://molmo.allenai.org.

https://molmo.allenai.org/blog

Allen AI의 멀티모달 모델. 이미지-텍스트 정렬에 사용할 캡션 데이터를 특이한 방법으로 모았네요.

일단 기존의 멀티모달 모델을 사용해서 생성하는 것은 피하려고 시도했습니다. 그런데 사람을 통해 수집하자니 작업이 쉽지 않아 선택한 것이 텍스트로 쓰는 대신 이미지에 대한 설명을 구술하게 했네요. 그리고 이를 ASR로 변환한 다음 LLM으로 텍스트를 교정했습니다.

SFT용으로는 시계 읽기나 Visual Grounding과 같은 과제들을 추가했군요. 평가에서도 15K의 이미지 쿼리들을 수집해 사람을 통해 평가했습니다.

상당히 공들인 프로젝트네요. 특히 텍스트로 쓰게 하는 대신 말로 설명하게 한다는 아이디어는 굉장히 흥미롭습니다.

#dataset #vision-language #captioning 