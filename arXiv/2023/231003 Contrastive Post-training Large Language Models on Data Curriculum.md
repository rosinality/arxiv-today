https://arxiv.org/abs/2310.02263

Contrastive Post-training Large Language Models on Data Curriculum (Canwen Xu, Corby Rosset, Luciano Del Corro, Shweti Mahajan, Julian McAuley, Jennifer Neville, Ahmed Hassan Awadallah, Nikhil Rao)

더 강한 모델(GPT-4)의 샘플을 positive, 더 약한 모델(GPT-3.5)의 샘플을 negative로 놓고 DPO나 SLiC 같은 offline 방법으로 학습시켰을 때 SFT 모델에 대해 향상이 있었다는 결과. 모델 크기로 synthetic reward를 만들었던 연구 (https://arxiv.org/abs/2305.13735) 가 생각나네요.

논문의 의도와는 다르겠지만 negative sample을 사용하는 것의 효과를 조금 보여주는 것이 아닌가 싶습니다.

#alignment

# Links

[[230523 Aligning Large Language Models through Synthetic Feedback.md]]