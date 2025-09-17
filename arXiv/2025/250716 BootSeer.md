https://arxiv.org/abs/2507.12619

*BootSeer: Analyzing and Mitigating Initialization Bottlenecks in Large-Scale LLM Training* (Rui Li, Xiaoyun Zhi, Jinxin Chi, Menghan Yu, Lixin Huang, Jia Zhu, Weilun Zhang, Xing Ma, Wenjia Liu, Zhicheng Zhu, Daowen Luo, Zuquan Song, Xin Yin, Chao Xiang, Shuguang Wang, Wencong Xiao, Gene Cooperman)

> Large Language Models (LLMs) have become a cornerstone of modern AI, driving breakthroughs in natural language processing and expanding into multimodal jobs involving images, audio, and video. As with most computational software, it is important to distinguish between ordinary runtime performance and startup overhead. Prior research has focused on runtime performance: improving training efficiency and stability. This work focuses instead on the increasingly critical issue of startup overhead in training: the delay before training jobs begin execution. Startup overhead is particularly important in large, industrial-scale LLMs, where failures occur more frequently and multiple teams operate in iterative update-debug cycles. In one of our training clusters, more than 3.5% of GPU time is wasted due to startup overhead alone. In this work, we present the first in-depth characterization of LLM training startup overhead based on real production data. We analyze the components of startup cost, quantify its direct impact, and examine how it scales with job size. These insights motivate the design of Bootseer, a system-level optimization framework that addresses three primary startup bottlenecks: (a) container image loading, (b) runtime dependency installation, and (c) model checkpoint resumption. To mitigate these bottlenecks, Bootseer introduces three techniques: (a) hot block record-and-prefetch, (b) dependency snapshotting, and (c) striped HDFS-FUSE. Bootseer has been deployed in a production environment and evaluated on real LLM training workloads, demonstrating a 50% reduction in startup overhead.

본격적인 학습 시작 전까지 걸리는 시간을 단축하기 위한 작업. 컨테이너를 어떻게 빨리 띄울 것인가, 체크포인트를 어떻게 더 빨리 불러올 것인가 같은 문제입니다.

<english>
Work for reducing startup time before actual training. It is problems like how can we initiate container faster, or load checkpoint faster.
</english>

#efficient-training 