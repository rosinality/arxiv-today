https://arxiv.org/abs/2402.13250

*Video ReCap: Recursive Captioning of Hour-Long Videos* (Md Mohaiminul Islam, Ngan Ho, Xitong Yang, Tushar Nagarajan, Lorenzo Torresani, Gedas Bertasius)

> Most video captioning models are designed to process short video clips of few seconds and output text describing low-level visual concepts (e.g., objects, scenes, atomic actions). However, most real-world videos last for minutes or hours and have a complex hierarchical structure spanning different temporal granularities. We propose Video ReCap, a recursive video captioning model that can process video inputs of dramatically different lengths (from 1 second to 2 hours) and output video captions at multiple hierarchy levels. The recursive video-language architecture exploits the synergy between different video hierarchies and can process hour-long videos efficiently. We utilize a curriculum learning training scheme to learn the hierarchical structure of videos, starting from clip-level captions describing atomic actions, then focusing on segment-level descriptions, and concluding with generating summaries for hour-long videos. Furthermore, we introduce Ego4D-HCap dataset by augmenting Ego4D with 8,267 manually collected long-range video summaries. Our recursive model can flexibly generate captions at different hierarchy levels while also being useful for other complex video understanding tasks, such as VideoQA on EgoSchema. Data, code, and models are available at: https://sites.google.com/view/vidrecap

긴 비디오에 대한 캡셔닝. 비디오를 짧게 쪼개서 그에 대해 캡셔닝을 하고, 비디오와 캡셔닝 결과를 합쳐 임베딩을 만든 다음 이 임베딩에 대해서 캡셔닝을 하는 것을 반복하는 형태입니다.

비디오를 통째로 학습시키는 방식을 채택하더라도 짧은 비디오에 대한 캡션을 조합해 긴 비디오에 대한 캡션을 만들도록 LLM을 튜닝해서 레이블을 만든 부분 등은 참고할만할 것 같네요.

#captioning #video