https://arxiv.org/abs/2311.17311

Universal Self-Consistency for Large Language Model Generation (Xinyun Chen, Renat Aksitov, Uri Alon, Jie Ren, Kefan Xiao, Pengcheng Yin, Sushant Prakash, Charles Sutton, Xuezhi Wang, Denny Zhou)

Self-Consistency는 흥미로운 방법이지만 voting을 하기에 응답이 일정한 형태여야 한다는 제약이 있었죠. 그래서 voting을 기계적으로 하는 대신 응답을 연결한 다음 LLM에 던져서 가장 consistent한 응답이 무엇인지를 출력하게 만들었습니다. 생성보다 검증이 쉽다. 특히 생성 결과가 여러 개 있는 경우에는, 이런 느낌이네요.

#prompt 