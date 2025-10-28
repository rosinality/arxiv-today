https://arxiv.org/abs/2510.20171

*Collective Communication for 100k+ GPUs* (Min Si, Pavan Balaji, Yongzhou Chen, Ching-Hsiang Chu, Adi Gangidi, Saif Hasan, Subodh Iyengar, Dan Johnson, Bingzhe Liu, Jingliang Ren, Ashmitha Jeevaraj Shetty, Greg Steinbrecher, Xinfeng Xie, Yulun Wang, Bruce Wu, Jingyi Yang, Mingran Yang, Minlan Yu, Cen Zhao, Wes Bland, Denis Boyda, Suman Gumudavelli, Cristian Lumezanu, Rui Miao, Zhe Qu, Venkat Ramesh, Maxim Samoylov, Jan Seidel, Feng Tian, Qiye Tan, Shuqiang Zhang, Yimeng Zhao, Shengbao Zheng, Art Zhu, Hongyi Zeng)

> The increasing scale of large language models (LLMs) necessitates highly efficient collective communication frameworks, particularly as training workloads extend to hundreds of thousands of GPUs. Traditional communication methods face significant throughput and latency limitations at this scale, hindering both the development and deployment of state-of-the-art models. This paper presents the NCCLX collective communication framework, developed at Meta, engineered to optimize performance across the full LLM lifecycle, from the synchronous demands of large-scale training to the low-latency requirements of inference. The framework is designed to support complex workloads on clusters exceeding 100,000 GPUs, ensuring reliable, high-throughput, and low-latency data exchange. Empirical evaluation on the Llama4 model demonstrates substantial improvements in communication efficiency. This research contributes a robust solution for enabling the next generation of LLMs to operate at unprecedented scales.

torchcomms의 NCCLX에 대한 리포트. NCCLX의 핵심은 완전히 새로운 전송 계층 (CTran).

NCCLX in torchcomms. The core of it was completely new transport layer (CTran).

#efficiency #parallelism 