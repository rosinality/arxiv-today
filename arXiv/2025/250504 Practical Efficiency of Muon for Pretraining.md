https://arxiv.org/abs/2505.02222

*Practical Efficiency of Muon for Pretraining* (Essential AI: Ishaan Shah, Anthony M. Polloreno, Karl Stratos, Philip Monk, Adarsh Chaluvaraju, Andrew Hojel, Andrew Ma, Anil Thomas, Ashish Tanwer, Darsh J Shah, Khoi Nguyen, Kurt Smith, Michael Callahan, Michael Pust, Mohit Parmar, Peter Rushton, Platon Mazarakis, Ritvik Kapila, Saurabh Srivastava, Somanshu Singla, Tim Romanski, Yash Vanjani, Ashish Vaswani)

> We demonstrate that Muon, the simplest instantiation of a second-order optimizer, explicitly expands the Pareto frontier over AdamW on the compute-time tradeoff. We find that Muon is more effective than AdamW in retaining data efficiency at large batch sizes, far beyond the so-called critical batch size, while remaining computationally efficient, thus enabling more economical training. We study the combination of Muon and the maximal update parameterization (muP) for efficient hyperparameter transfer and present a simple telescoping algorithm that accounts for all sources of error in muP while introducing only a modest overhead in resources. We validate our findings through extensive experiments with model sizes up to four billion parameters and ablations on the data distribution and architecture.

Muon과 Muon를 위한 muP에 대한 분석. 실험 규모가 크진 않은데 15% 정도의 데이터 효율성 증가를 이야기하고 있네요.

Essential AI가 어떤 회사인가 했는데 Ashish Vaswani가 창립한 회사군요.

<english>
Analysis on Muon and muP for Muon. Scale of experiments are not very large, while reports 15% increase of data efficiency.

I wounder what company Essential AI is, and it was a company founded by Ashish Vaswani.
</english>

#optimizer #hyperparameter 