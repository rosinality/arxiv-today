https://arxiv.org/abs/2504.20879

*The Leaderboard Illusion* (Shivalika Singh, Yiyang Nan, Alex Wang, Daniel D'Souza, Sayash Kapoor, Ahmet Üstün, Sanmi Koyejo, Yuntian Deng, Shayne Longpre, Noah Smith, Beyza Ermis, Marzieh Fadaee, Sara Hooker)

> Measuring progress is fundamental to the advancement of any scientific field. As benchmarks play an increasingly central role, they also grow more susceptible to distortion. Chatbot Arena has emerged as the go-to leaderboard for ranking the most capable AI systems. Yet, in this work we identify systematic issues that have resulted in a distorted playing field. We find that undisclosed private testing practices benefit a handful of providers who are able to test multiple variants before public release and retract scores if desired. We establish that the ability of these providers to choose the best score leads to biased Arena scores due to selective disclosure of performance results. At an extreme, we identify 27 private LLM variants tested by Meta in the lead-up to the Llama-4 release. We also establish that proprietary closed models are sampled at higher rates (number of battles) and have fewer models removed from the arena than open-weight and open-source alternatives. Both these policies lead to large data access asymmetries over time. Providers like Google and OpenAI have received an estimated 19.2% and 20.4% of all data on the arena, respectively. In contrast, a combined 83 open-weight models have only received an estimated 29.7% of the total data. We show that access to Chatbot Arena data yields substantial benefits; even limited additional data can result in relative performance gains of up to 112% on the arena distribution, based on our conservative estimates. Together, these dynamics result in overfitting to Arena-specific dynamics rather than general model quality. The Arena builds on the substantial efforts of both the organizers and an open community that maintains this valuable evaluation platform. We offer actionable recommendations to reform the Chatbot Arena's evaluation framework and promote fairer, more transparent benchmarking for the field

Chatbot Arena에서 비공개로 모델을 테스트한 다음 모델을 조용히 제외시키는 풍조에 대한 비판. 3월 한 달에만 메타가 27개 모델을 비공개 평가했군요. 평가한 다음 선택적으로 모델을 제외시키는 것으로 순위를 바꾸고 수집한 데이터로 리더보드에 오버피팅 하는 것이 가능하죠.

벤치마크는 모델을 잘 만든 다음 그걸 평가하기 위한 것이어야 하죠. 벤치마크를 타겟하기 시작하면 언제나 문제가 발생합니다.

<english>
Criticism on trend of testing silently retracting privative models in Chatbot Arena. Meta privately tested 27 models on March alone. After evaluating they are able to change ranks by selectively retracting and can do overfitting using collected data.

Benchmark should be a measure of evaluation after build model well. Targeting benchmarks itself alwas causes a problem.
</english>

#benchmark 