https://arxiv.org/abs/2510.11495

*How Reinforcement Learning After Next-Token Prediction Facilitates Learning* (Nikolaos Tsilivis, Eran Malach, Karen Ullrich, Julia Kempe)

> Recent advances in reasoning domains with neural networks have primarily been enabled by a training recipe that optimizes Large Language Models, previously trained to predict the next-token in a sequence, with reinforcement learning algorithms. We introduce a framework to study the success of this paradigm, and we theoretically expose the optimization mechanisms by which reinforcement learning improves over next-token prediction in this setting. We study learning from mixture distributions of short and long ``chain-of-thought'' sequences encoding a single task. In particular, when the task consists of predicting the parity of $d$ bits and long sequences are rare, we show how reinforcement learning after next-token prediction enables autoregressive transformers to generalize, whereas mere next-token prediction requires extreme statistical or computational resources to do so. We further explain how reinforcement learning leverages increased test-time computation, manifested in longer responses, to facilitate this learning process. In a simplified setting, we theoretically prove that autoregressive linear models following this training recipe can efficiently learn to predict the parity of $d$ bits as long as the proportion of long demonstrations in the data mix is not exponentially small in the input dimension $d$. Finally, we demonstrate these same phenomena in other settings, including the post-training of Llama-series models on mixture variations of common mathematical reasoning benchmarks.

<english>
Why RL after pretraining is so effective? RL upsamples the generalizable-but-rare patterns in the pretrained model.
</english>

#rl #generalization #reasoning 