https://arxiv.org/abs/2310.08754

Tokenizer Choice For LLM Training: Negligible or Crucial? (Mehdi Ali, Michael Fromm, Klaudia Thellmann, Richard Rutmann, Max Lübbering, Johannes Leveling, Katrin Klug, Jan Ebert, Niclas Doll, Jasper Schulze Buschhoff, Charvi Jain, Alexander Arno Weber, Lena Jurkschat, Hammam Abdelwahab, Chelsea John, Pedro Ortiz Suarez, Malte Ostendorff, Samuel Weinbach, Rafet Sifa, Stefan Kesselheim, Nicolas Flores-Herr)

토크나이저 비교 분석. monolingual/multilingual 상황에서 BPE vs Unigram과 HuggingFace vs SentencePiece, vocab 수 등에 대해 fertility와 parity (서로 다른 언어의 토큰화 이후 길이 차이 비교) 같은 intrinsic metric과 downstream task에 대한 비교 결과를 봤습니다.

downstream task에 대한 차이는 미묘한 것 같아서 fertility가 꽤 괜찮은 지표일지도 모르겠다는 생각이 드네요. 그렇지만 조금이라도 나은 결과가 나온 세팅을 채택하는 것은 괜찮겠죠. 여담이지만 영어는 33K vocab 정도로 충분하다는 것 같습니다.

#tokenizer 