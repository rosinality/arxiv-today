https://arxiv.org/abs/2505.10527

*WorldPM: Scaling Human Preference Modeling* (Binghai Wang, Runji Lin, Keming Lu, Le Yu, Zhenru Zhang, Fei Huang, Chujie Zheng, Kai Dang, Yang Fan, Xingzhang Ren, An Yang, Binyuan Hui, Dayiheng Liu, Tao Gui, Qi Zhang, Xuanjing Huang, Yu-Gang Jiang, Bowen Yu, Jingren Zhou, Junyang Lin)

> Motivated by scaling laws in language modeling that demonstrate how test loss scales as a power law with model and dataset sizes, we find that similar laws exist in preference modeling. We propose World Preference Modeling$ (WorldPM) to emphasize this scaling potential, where World Preference embodies a unified representation of human preferences. In this paper, we collect preference data from public forums covering diverse user communities, and conduct extensive training using 15M-scale data across models ranging from 1.5B to 72B parameters. We observe distinct patterns across different evaluation metrics: (1) Adversarial metrics (ability to identify deceptive features) consistently scale up with increased training data and base model size; (2) Objective metrics (objective knowledge with well-defined answers) show emergent behavior in larger language models, highlighting WorldPM's scalability potential; (3) Subjective metrics (subjective preferences from a limited number of humans or AI) do not demonstrate scaling trends. Further experiments validate the effectiveness of WorldPM as a foundation for preference fine-tuning. Through evaluations on 7 benchmarks with 20 subtasks, we find that WorldPM broadly improves the generalization performance across human preference datasets of varying sizes (7K, 100K and 800K samples), with performance gains exceeding 5% on many key subtasks. Integrating WorldPM into our internal RLHF pipeline, we observe significant improvements on both in-house and public evaluation sets, with notable gains of 4% to 8% in our in-house evaluations.

인터넷 포럼 데이터를 사용한 Reward Model 학습. 논문에서도 언급하지만 정확하게 Preference Model Pretraining이군요. 여기서는 PMP의 규모를 증대시켰을 때 나타나는 현상에 집중하고 있네요.

선호란 기준에 따라 다른 것이니 그 부분에서의 충돌이 있네요. 그리고 PMP 과정에서 Loss가 급격히 낮아지는 통찰의 순간이 발생했다는 이야기도 흥미롭습니다.

<english>
Training reward model using internet forum data. As mentioned in the paper, it is accurately preference model pretraining. This paper focus on the phenomena that occurs when scaling PMP.

As preference depends on the criteria, there are conflict in that aspect. And reported on occuring of moment of epiphany that sudden decrease of loss is also interesting.
</english>

#reward-model 