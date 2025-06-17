https://arxiv.org/abs/2504.04022

*Rethinking Reflection in Pre-Training* (Essential AI: Darsh J Shah, Peter Rushton, Somanshu Singla, Mohit Parmar, Kurt Smith, Yash Vanjani, Ashish Vaswani, Adarsh Chaluvaraju, Andrew Hojel, Andrew Ma, Anil Thomas, Anthony Polloreno, Ashish Tanwer, Burhan Drak Sibai, Divya S Mansingka, Divya Shivaprasad, Ishaan Shah, Karl Stratos, Khoi Nguyen, Michael Callahan, Michael Pust, Mrinal Iyer, Philip Monk, Platon Mazarakis, Ritvik Kapila, Saurabh Srivastava, Tim Romanski)

> A language model's ability to reflect on its own reasoning provides a key advantage for solving complex problems. While most recent research has focused on how this ability develops during reinforcement learning, we show that it actually begins to emerge much earlier - during the model's pre-training. To study this, we introduce deliberate errors into chains-of-thought and test whether the model can still arrive at the correct answer by recognizing and correcting these mistakes. By tracking performance across different stages of pre-training, we observe that this self-correcting ability appears early and improves steadily over time. For instance, an OLMo2-7B model pre-trained on 4 trillion tokens displays self-correction on our six self-reflection tasks.

오류가 있는 CoT에 대해 Wait 같은 키워드로 오류 수정을 유도했을 때 오류를 수정하는 능력이 프리트레이닝 연산량에 따라 증가한다는 분석. 프리트레이닝과 추론 포스트트레이닝의 관계를 좀 더 잘 이해하는 것이 앞으로 중요하겠죠.

<english>
The analysis insists that ability to error correction when model is given errorneous CoT and induce error correction behavior using keywords like Wait is increases with pretraining computes. It will be important to understand relationships between pretraining and reasoning post-training.
</english>

#scaling-law #reasoning 