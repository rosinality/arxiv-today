https://arxiv.org/abs/2401.13311

*ConTextual: Evaluating Context-Sensitive Text-Rich Visual Reasoning in Large Multimodal Models* (Rohan Wadhawan, Hritik Bansal, Kai-Wei Chang, Nanyun Peng)

> Recent advancements in AI have led to the development of large multimodal models (LMMs) capable of processing complex tasks involving joint reasoning over text and visual content in the image (e.g., navigating maps in public places). This paper introduces ConTextual, a novel benchmark comprising instructions designed explicitly to evaluate LMMs' ability to perform context-sensitive text-rich visual reasoning. ConTextual emphasizes diverse real-world scenarios (e.g., time-reading, navigation, shopping and more) demanding a deeper understanding of the interactions between textual and visual elements. Our findings reveal a significant performance gap of 30.8% between the best-performing LMM, GPT-4V(ision), and human capabilities using human evaluation indicating substantial room for improvement in context-sensitive text-rich visual reasoning. Notably, while GPT-4V excelled in abstract categories like meme and quote interpretation, its overall performance still lagged behind humans. In addition to human evaluations, we also employed automatic evaluation metrics using GPT-4, uncovering similar trends in performance disparities. We also perform a fine-grained evaluation across diverse visual contexts and provide qualitative analysis which provides a robust framework for future advancements in the LMM design. https://con-textual.github.io/

텍스트가 많이 포함된 이미지를 골라 텍스트만으로는 대답할 수 없는 문제로 구성한 벤치마크입니다. OCR로 텍스트만 추출할 수 있으면 풀 수 있는 것이 아니라 이미지 내 다른 구성 요소와의 관계를 고려하는 것이 중요한 사례들이라고 할 수 있겠네요.

모델에게 꽤 난이도가 있는 것으로 보이긴 합니다. 프롬프팅으로 푸는 사례들도 나오겠지만요.

#benchmark #vision-language #ocr 