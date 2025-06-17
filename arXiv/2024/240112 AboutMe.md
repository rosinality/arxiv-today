https://arxiv.org/abs/2401.06408

*AboutMe: Using Self-Descriptions in Webpages to Document the Effects of English Pretraining Data Filters* (Li Lucy, Suchin Gururangan, Luca Soldaini, Emma Strubell, David Bamman, Lauren Klein, Jesse Dodge)

> Large language models' (LLMs) abilities are drawn from their pretraining data, and model development begins with data curation. However, decisions around what data is retained or removed during this initial stage is under-scrutinized. In our work, we ground web text, which is a popular pretraining data source, to its social and geographic contexts. We create a new dataset of 10.3 million self-descriptions of website creators, and extract information about who they are and where they are from: their topical interests, social roles, and geographic affiliations. Then, we conduct the first study investigating how ten "quality" and English language identification (langID) filters affect webpages that vary along these social dimensions. Our experiments illuminate a range of implicit preferences in data curation: we show that some quality classifiers act like topical domain filters, and langID can overlook English content from some regions of the world. Overall, we hope that our work will encourage a new line of research on pretraining data curation practices and its social implications.

굉장히 흥미로운 분석이네요. 프리트레이닝 코퍼스에 적용되는 필터링 방식들(분류기, n-gram LM, 휴리스틱, 언어 분류기 등)이 적용되었을 때 어떤 종류의 문서들을 채택하고 어떤 종류의 문서를 필터링하는지를 분석했습니다.

문서의 종류를 판단하기 위해 웹사이트의 About 페이지를 활용했다는 것도 재미있네요. 분석 결과 쇼핑몰과 동시에 예술 같은 시각적인 페이지가 걸러진다는 것, 단체보다는 개인의 웹사이트가 채택된다는 것, 선호되는 직업들과 지역, 그리고 이런 패턴이 필터링 방법에 따라 어떻게 달라지는지를 관찰했습니다.

필터링 방법들이 꽤 의도대로 작동하고 있다는 생각은 듭니다. (쇼핑몰 페이지들을 거른다는 것 등.) 다만 그렇더라도 프리트레이닝 코퍼스 필터링에 채택하고 있는 방법들과 파이프라인 전반이 어떤 페이지들을 필터링하는지를 좀 더 확인해보는 것은 검증 차원에서도 의미 있겠다 싶네요.

#corpus 