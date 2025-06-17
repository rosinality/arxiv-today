https://arxiv.org/abs/2408.17003

*Safety Layers of Aligned Large Language Models: The Key to LLM Security* (Shen Li, Liuyi Yao, Lan Zhang, Yaliang Li)

> Aligned LLMs are highly secure, capable of recognizing and refusing to answer malicious questions. However, the role of internal parameters in maintaining this security is not well understood, further these models are vulnerable to security degradation when fine-tuned with non-malicious backdoor data or normal data. To address these challenges, our work uncovers the mechanism behind security in aligned LLMs at the parameter level, identifying a small set of contiguous layers in the middle of the model that are crucial for distinguishing malicious queries from normal ones, referred to as "safety layers." We first confirm the existence of these safety layers by analyzing variations in input vectors within the model's internal layers. Additionally, we leverage the over-rejection phenomenon and parameters scaling analysis to precisely locate the safety layers. Building on this understanding, we propose a novel fine-tuning approach, Safely Partial-Parameter Fine-Tuning (SPPFT), that fixes the gradient of the safety layers during fine-tuning to address the security degradation. Our experiments demonstrate that this approach significantly preserves model security while maintaining performance and reducing computational resources compared to full fine-tuning.

정렬된 LLM에서 Safety를 담당하는 레이어 찾기. LLM이 흔히 그렇듯 중간 단계에 위치하고 있습니다. 초기 레이어는 문법적인 특징들을 추출하기 바쁘고 후기 레이어는 출력 결과를 생성하기 바쁜 것이겠죠.

#safety #alignment #mechanistic-interpretation 