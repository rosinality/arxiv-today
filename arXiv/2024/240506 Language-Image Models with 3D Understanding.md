https://arxiv.org/abs/2405.03685

*Language-Image Models with 3D Understanding* (Jang Hyun Cho, Boris Ivanovic, Yulong Cao, Edward Schmerling, Yue Wang, Xinshuo Weng, Boyi Li, Yurong You, Philipp Krähenbühl, Yan Wang, Marco Pavone)

> Multi-modal large language models (MLLMs) have shown incredible capabilities in a variety of 2D vision and language tasks. We extend MLLMs' perceptual capabilities to ground and reason about images in 3-dimensional space. To that end, we first develop a large-scale pre-training dataset for 2D and 3D called LV3D by combining multiple existing 2D and 3D recognition datasets under a common task formulation: as multi-turn question-answering. Next, we introduce a new MLLM named Cube-LLM and pre-train it on LV3D. We show that pure data scaling makes a strong 3D perception capability without 3D specific architectural design or training objective. Cube-LLM exhibits intriguing properties similar to LLMs: (1) Cube-LLM can apply chain-of-thought prompting to improve 3D understanding from 2D context information. (2) Cube-LLM can follow complex and diverse instructions and adapt to versatile input and output formats. (3) Cube-LLM can be visually prompted such as 2D box or a set of candidate 3D boxes from specialists. Our experiments on outdoor benchmarks demonstrate that Cube-LLM significantly outperforms existing baselines by 21.3 points of AP-BEV on the Talk2Car dataset for 3D grounded reasoning and 17.7 points on the DriveLM dataset for complex reasoning about driving scenarios, respectively. Cube-LLM also shows competitive results in general MLLM benchmarks such as refCOCO for 2D grounding with (87.0) average score, as well as visual question answering benchmarks such as VQAv2, GQA, SQA, POPE, etc. for complex reasoning. Our project is available at https://janghyuncho.github.io/Cube-LLM.

박스와 포인트 레이블을 사용해서 학습한 3D Aware LLM. LLM처럼 하나의 Objective로 "알아서" 이미지의 모든 특성을 추출할 수 있다면, 그리고 마찬가지로 "알아서" 이미지와 텍스트, 그리고 텍스트로 표현 가능한 모든 과제를 연결할 수 있다면 어떨까 하는 생각을 합니다. 다만 어쩌면 이미지에 대해서는 수많은 과제를 통해 접근하는 것이 나은 방법일지도 모르겠네요. (https://arxiv.org/abs/2312.00785) 또는 비디오가 문제를 모두 해결해줄 수도 있겠죠. 앞으로 어떻게 흘러갈지 궁금한 문제입니다.

#vision-language #3d

# Links

[[231201 Sequential Modeling Enables Scalable Learning for Large Vision Models.md]]