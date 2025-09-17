https://arxiv.org/abs/2509.07963

*Customizing the Inductive Biases of Softmax Attention using Structured Matrices* (Yilun Kuang, Noah Amsel, Sanae Lotfi, Shikai Qiu, Andres Potapczynski, Andrew Gordon Wilson)

> The core component of attention is the scoring function, which transforms the inputs into low-dimensional queries and keys and takes the dot product of each pair. While the low-dimensional projection improves efficiency, it causes information loss for certain tasks that have intrinsically high-dimensional inputs. Additionally, attention uses the same scoring function for all input pairs, without imposing a distance-dependent compute bias for neighboring tokens in the sequence. In this work, we address these shortcomings by proposing new scoring functions based on computationally efficient structured matrices with high ranks, including Block Tensor-Train (BTT) and Multi-Level Low Rank (MLR) matrices. On in-context regression tasks with high-dimensional inputs, our proposed scoring functions outperform standard attention for any fixed compute budget. On language modeling, a task that exhibits locality patterns, our MLR-based attention method achieves improved scaling laws compared to both standard attention and variants of sliding window attention. Additionally, we show that both BTT and MLR fall under a broader family of efficient structured matrices capable of encoding either full-rank or distance-dependent compute biases, thereby addressing significant shortcomings of standard attention. Finally, we show that MLR attention has promising results for long-range time-series forecasting.

Attention Score x^TQK^Tx에 대해 구조화된 행렬을 사용해 Rank를 증가시키고 Locality Bias를 주입. 그런데 GPU에서 효율적인 구현이 가능할지?

Using structured matrices for attention scores x^TQK^Tx to increase rank and inject locality bias. But can this be efficiently implemented on GPUs?

#attention 