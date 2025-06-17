https://arxiv.org/abs/2411.00284

*SimpleFSDP: Simpler Fully Sharded Data Parallel with torch.compile* (Ruisi Zhang, Tianyu Liu, Will Feng, Andrew Gu, Sanket Purandare, Wanchao Liang, Francisco Massa)

> Distributed training of large models consumes enormous computation resources and requires substantial engineering efforts to compose various training techniques. This paper presents SimpleFSDP, a PyTorch-native compiler-based Fully Sharded Data Parallel (FSDP) framework, which has a simple implementation for maintenance and composability, allows full computation-communication graph tracing, and brings performance enhancement via compiler backend optimizations. SimpleFSDP's novelty lies in its unique torch.compile-friendly implementation of collective communications using existing PyTorch primitives, namely parametrizations, selective activation checkpointing, and DTensor. It also features the first-of-its-kind intermediate representation (IR) nodes bucketing and reordering in the TorchInductor backend for effective computation-communication overlapping. As a result, users can employ the aforementioned optimizations to automatically or manually wrap model components for minimal communication exposure. Extensive evaluations of SimpleFSDP on Llama 3 models (including the ultra-large 405B) using TorchTitan demonstrate up to 28.54% memory reduction and 68.67% throughput improvement compared to the most widely adopted FSDP2 eager framework, when composed with other distributed training techniques.

새로운 PyTorch FSDP 구현이군요. DTensor를 기반으로 TorchInductor에 통신 최적화를 위한 Bucketing과 Reordering을 추가하는 형태로 구현됐습니다. Jax와 보다 비슷한 느낌이 됐네요.

<english>
New FSDP implementation in PyTorch. It is implemented based on DTensor with communication optimizations by bucketing and reordering in TorchInductor. It is much similar to Jax now.
</english>

#efficiency #parallelism 