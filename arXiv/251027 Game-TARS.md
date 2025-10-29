https://arxiv.org/abs/2510.23691

*Game-TARS: Pretrained Foundation Models for Scalable Generalist Multimodal Game Agents* (Zihao Wang, Xujing Li, Yining Ye, Junjie Fang, Haoming Wang, Longxiang Liu, Shihao Liang, Junting Lu, Zhiyong Wu, Jiazhan Feng, Wanjun Zhong, Zili Li, Yu Wang, Yu Miao, Bo Zhou, Yuanfan Li, Hao Wang, Zhongkai Zhao, Faming Wu, Zhengxuan Jiang, Weihao Tan, Heyuan Yao, Shi Yan, Xiangyang Li, Yitao Liang, Yujia Qin, Guang Shi)

> We present Game-TARS, a generalist game agent trained with a unified, scalable action space anchored to human-aligned native keyboard-mouse inputs. Unlike API- or GUI-based approaches, this paradigm enables large-scale continual pre-training across heterogeneous domains, including OS, web, and simulation games. Game-TARS is pre-trained on over 500B tokens with diverse trajectories and multimodal data. Key techniques include a decaying continual loss to reduce causal confusion and an efficient Sparse-Thinking strategy that balances reasoning depth and inference cost. Experiments show that Game-TARS achieves about 2 times the success rate over the previous sota model on open-world Minecraft tasks, is close to the generality of fresh humans in unseen web 3d games, and outperforms GPT-5, Gemini-2.5-Pro, and Claude-4-Sonnet in FPS benchmarks. Scaling results on training-time and test-time confirm that the unified action space sustains improvements when scaled to cross-game and multimodal data. Our results demonstrate that simple, scalable action representations combined with large-scale pre-training provide a promising path toward generalist agents with broad computer-use abilities.

게임 에이전트에 대한 프리, 포스트트레이닝. 키보드와 마우스 입력을 포함한 20K 시간의 게임 플레이를 수집. 생각의 과정도 수집하기 위해 Think-aloud를 시켰음 (!)

Pre and post-training of a game agent. They collected 20K hours of gameplay data with keyboard and mouse inputs, and think-aloud (!) for thought trajectory.

#pretraining #agent #post-training 