https://arxiv.org/abs/2404.07449

*Learning to Localize Objects Improves Spatial Reasoning in Visual-LLMs* (Kanchana Ranasinghe, Satya Narayan Shukla, Omid Poursaeed, Michael S. Ryoo, Tsung-Yu Lin)

> Integration of Large Language Models (LLMs) into visual domain tasks, resulting in visual-LLMs (V-LLMs), has enabled exceptional performance in vision-language tasks, particularly for visual question answering (VQA). However, existing V-LLMs (e.g. BLIP-2, LLaVA) demonstrate weak spatial reasoning and localization awareness. Despite generating highly descriptive and elaborate textual answers, these models fail at simple tasks like distinguishing a left vs right location. In this work, we explore how image-space coordinate based instruction fine-tuning objectives could inject spatial awareness into V-LLMs. We discover optimal coordinate representations, data-efficient instruction fine-tuning objectives, and pseudo-data generation strategies that lead to improved spatial awareness in V-LLMs. Additionally, our resulting model improves VQA across image and video domains, reduces undesired hallucination, and generates better contextual object descriptions. Experiments across 5 vision-language tasks involving 14 different datasets establish the clear performance improvements achieved by our proposed framework.

Visual Grounding이나 지정한 위치를 기술하도록 하는 Location 관련 과제를 학습시키면 공간적 추론 능력이 향상된다는 결과.

Vision Language 모델에서 이미지에 포함된 정보를 최대한 추출하도록 하려면 다양한 이미지 관련 과제들이 학습에 포함되어야 하는 것이 아닌가 하는 생각이 있습니다. 다만 이쪽은 한 가지 Objective로 Unsupervised Training을 한다고 하는 텍스트에 대한 학습과는 전혀 다른 방향이죠. 이 차이를 해소할 수 있다면 재미있지 않을까 싶습니다.

이미지나 텍스트 자체에 대한 Unsupervised Training이 각 모달리티에 대해서 풍성한 구조를 추출해낼 수 있겠지만, 이 둘을 잇는 Alignment 과정에서의 Caption Generation은 이미지에 대해서 할 수 있는 수많은 과제 중 하나에 그친다는 것이 문제일지도 모르겠습니다. 물론 Captioning이 가지는 다양성도 아주 크긴 하지만요. 전 이미지에 포함된 밀집된 정보에 비해 언어에 포함된 정보는 성긴 경우가 많다고 봅니다. (물론 이것도 의견이 달라서 텍스트에 비해 이미지는 정보량이 적다고 생각하는 사람들도 있더군요. 용량으로 따지면 그럴지도 모르겠습니다.)

#vision-language #visual-grounding 