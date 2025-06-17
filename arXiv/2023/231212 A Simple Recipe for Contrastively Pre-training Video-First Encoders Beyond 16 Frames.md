https://arxiv.org/abs/2312.07395

A Simple Recipe for Contrastively Pre-training Video-First Encoders Beyond 16 Frames (Pinelopi Papalampidi, Skanda Koppula, Shreya Pathak, Justin Chiu, Joe Heyward, Viorica Patraucean, Jiajun Shen, Antoine Miech, Andrew Zisserman, Aida Nematzdeh)

(이미지도 해상도가 높아지면 그렇지만) 비디오는 정말 토큰 싸움(?)이군요. 이미지와 짧은 영상 -> 긴 영상 순서로 Video-Language Contrastive Pretraining을 하고 Temporal Pooling에 Perceiver로 Resample, Token masking에 PEFT가 들어갔네요. 결과적으로는 심플한 게 맞나 싶긴 합니다. 어쩔 수 없는 점이 있지만요.

#video_transformer #contrastive_learning 