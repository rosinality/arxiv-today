https://arxiv.org/abs/2505.11441

*Is Compression Really Linear with Code Intelligence?* (Xianzhen Luo, Shijie Xuyang, Tianhao Cheng, Zheng Chu, Houyi Li, ziqi wang, Siming Huang, Qingfu Zhu, Qiufeng Wang, Xiangyu Zhang, Shuigeng Zhou, Wanxiang Che)

> Understanding the relationship between data compression and the capabilities of Large Language Models (LLMs) is crucial, especially in specialized domains like code intelligence. Prior work posited a linear relationship between compression and general intelligence. However, it overlooked the multifaceted nature of code that encompasses diverse programming languages and tasks, and struggled with fair evaluation of modern Code LLMs. We address this by evaluating a diverse array of open-source Code LLMs on comprehensive multi-language, multi-task code benchmarks. To address the challenge of efficient and fair evaluation of pre-trained LLMs' code intelligence, we introduce \textit{Format Annealing}, a lightweight, transparent training methodology designed to assess the intrinsic capabilities of these pre-trained models equitably. Compression efficacy, measured as bits-per-character (BPC), is determined using a novel, large-scale, and previously unseen code validation set derived from GitHub. Our empirical results reveal a fundamental logarithmic relationship between measured code intelligence and BPC. This finding refines prior hypotheses of linearity, which we suggest are likely observations of the logarithmic curve's tail under specific, limited conditions. Our work provides a more nuanced understanding of compression's role in developing code intelligence and contributes a robust evaluation framework in the code domain.

코드 BPC와 과제 성능과의 관계. 이를 위해 벤치마크 셋을 구성하고 평가시 포맷 문제를 해소하기 위한 튜닝 절차를 만들었군요.

<english>
Relationship of code BPE and downstream task performance. For this they constructed benchmarks and tuning steps for reducing format related issues.
</english>

#code #scaling-law 