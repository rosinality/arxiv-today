https://arxiv.org/abs/2505.24832

*How much do language models memorize?* (John X. Morris, Chawin Sitawarin, Chuan Guo, Narine Kokhlikyan, G. Edward Suh, Alexander M. Rush, Kamalika Chaudhuri, Saeed Mahloujifar)

> We propose a new method for estimating how much a model ``knows'' about a datapoint and use it to measure the capacity of modern language models. Prior studies of language model memorization have struggled to disentangle memorization from generalization. We formally separate memorization into two components: \textit{unintended memorization}, the information a model contains about a specific dataset, and \textit{generalization}, the information a model contains about the true data-generation process. When we completely eliminate generalization, we can compute the total memorization, which provides an estimate of model capacity: our measurements estimate that GPT-style models have a capacity of approximately 3.6 bits per parameter. We train language models on datasets of increasing size and observe that models memorize until their capacity fills, at which point ``grokking'' begins, and unintended memorization decreases as models begin to generalize. We train hundreds of transformer language models ranging from $500K$ to $1.5B$ parameters and produce a series of scaling laws relating model capacity and data size to membership inference.

트랜스포머의 저장 공간에 대한 분석. 데이터의 규모가 저장 공간을 모두 채우는 이상의 시점이 되면 일반화 경향이 등장하기 시작한다고.

<english>
Analysis on memorization capacity of transformer. It suggest that generalization appears when scale of data is became larger than memorization capacity of the model.
</english>

#scaling-law #llm 