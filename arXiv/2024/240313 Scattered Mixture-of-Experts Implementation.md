https://arxiv.org/abs/2403.08245

*Scattered Mixture-of-Experts Implementation* (Shawn Tan, Yikang Shen, Rameswar Panda, Aaron Courville)

> We present ScatterMoE, an implementation of Sparse Mixture-of-Experts (SMoE) on GPUs. ScatterMoE builds upon existing implementations, and overcoming some of the limitations to improve inference and training speed, and memory footprint. This implementation achieves this by avoiding padding and making excessive copies of the input. We introduce ParallelLinear, the main component we use to build our implementation and the various kernels used to speed up the operation. We benchmark our implementation against Megablocks, and show that it enables a higher throughput and lower memory footprint. We also show how ParallelLinear enables extension of the Mixture-of-Experts concept by demonstrating with an implementation of Mixture of Attention.

