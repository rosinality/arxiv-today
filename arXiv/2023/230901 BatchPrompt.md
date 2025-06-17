https://arxiv.org/abs/2309.00384

BatchPrompt: Accomplish more with less (Jianzhe Lin, Maurice Diesendruck, Liang Du, Robin Abraham)

각 데이터 샘플보다 프롬프트가 더 길어지면 배 보다 배꼽이 더 커지는 격이니 데이터를 여럿 묶어 배치화하면 좋겠다는 아이디어. 그런데 그냥 묶어서 한 번에 처리하면 성능이 떨어지니 샘플 순서를 섞어 여러 번 호출한 다음 voting을 결합. 사실 API의 제약에 대한 우회라고 보이긴 하네요.

#efficiency 