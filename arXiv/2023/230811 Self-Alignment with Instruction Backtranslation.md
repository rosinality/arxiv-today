https://arxiv.org/abs/2308.06259

Self-Alignment with Instruction Backtranslation (Xian Li, Ping Yu, Chunting Zhou, Timo Schick, Luke Zettlemoyer, Omer Levy, Jason Weston, Mike Lewis)

Alignment를 위한 sft 데이터 구축 방법. 3K 정도의 시드 데이터를 사용해서 unlabeled corpus에서 instruction을 생성하는 모델을 만들고, 이렇게 만든 pair들을 스코어링해서 필터링하는 방식으로 데이터를 구축하는 군요. 여러모로 instruction following 능력을 살짝 탑재하면 그 이후는 자동화된 방식으로 개선하는 것이 가능해 보이네요.포맷 등의 측면에서 한계가 있지 않을까 하는 생각은 들지만 충분히 유망해 보입니다. 나머지는 rlhf로 개선하는 것도 가능할 수 있겠네요.

[[221215 Constitutional AI]] instruction 생성만이 아니라 본문의 개선 또한 가능할까?

#alignment #instruction-tuning 