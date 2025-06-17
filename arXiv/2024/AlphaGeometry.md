https://www.nature.com/articles/s41586-023-06747-5

*Solving olympiad geometry without human demonstrations* (Trie H. Trinh, Yukuai Wu, Quoc V. Le, He He, Thang Luong)

> Proving mathematical theorems at the olympiad level represents a notable milestone in human-level automated reasoning, owing to their reputed difficulty among the world’s best talents in pre-university mathematics. Current machine-learning approaches, however, are not applicable to most mathematical domains owing to the high cost of translating human proofs into machine-verifiable format. The problem is even worse for geometry because of its unique translation challenges, resulting in severe scarcity of training data. We propose AlphaGeometry, a theorem prover for Euclidean plane geometry that sidesteps the need for human demonstrations by synthesizing millions of theorems and proofs across different levels of complexity. AlphaGeometry is a neuro-symbolic system that uses a neural language model, trained from scratch on our large-scale synthetic data, to guide a symbolic deduction engine through infinite branching points in challenging problems. On a test set of 30 latest olympiad-level problems, AlphaGeometry solves 25, outperforming the previous best method that only solves ten problems and approaching the performance of an average International Mathematical Olympiad (IMO) gold medallist. Notably, AlphaGeometry produces human-readable proofs, solves all geometry problems in the IMO 2000 and 2015 under human expert evaluation and discovers a generalized version of a translated IMO theorem in 2004.

https://deepmind.google/discover/blog/alphageometry-an-olympiad-level-ai-system-for-geometry/
https://github.com/google-deepmind/alphageometry

딥마인드의 올림피아드 기하학 문제를 푸는 시스템. LM이 정의를 만들고 기호 기반 엔진이 전제와 정의로부터 결론들을 연역해나가는 것을 반복해서 증명에 도달해나가는 방법이군요.

데이터 전체를 합성해서 만들었는데 이 데이터의 구성 과정이 핵심이라고 할 수 있겠네요. 전제를 랜덤 샘플한 다음 이 전제에서 유도되는 결론들을 연역하고 이 연역 과정을 기반으로 결론들의 그래프를 만듭니다. 이렇게 하면 임의의 문제와 그에 대한 답을 생성하는 것이 되죠.

여기서 증명 시스템을 만들기 위해서는 정의를 생성할 수 있어야 하는데 이 정의는 결론에 포함되지 않지만 그래프에는 포함된 전제들을 사용합니다. 전제와 결론을 주고 정의들을 예측하게 만드는 것이죠. (이 부분이 좀 헷갈리긴 합니다.)

#search #symbolic
