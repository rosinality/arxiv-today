https://arxiv.org/abs/2406.11704

*Nemotron-4 340B Technical Report* (Nvidia: Bo Adler, Niket Agarwal, Ashwath Aithal, Dong H. Anh, Pallab Bhattacharya, Annika Brundyn, Jared Casper, Bryan Catanzaro, Sharon Clay, Jonathan Cohen, Sirshak Das, Ayush Dattagupta, Olivier Delalleau, Leon Derczynski, Yi Dong, Daniel Egert, Ellie Evans, Aleksander Ficek, Denys Fridman, Shaona Ghosh, Boris Ginsburg, Igor Gitman, Tomasz Grzegorzek, Robert Hero, Jining Huang, Vibhu Jawa, Joseph Jennings, Aastha Jhunjhunwala, John Kamalu, Sadaf Khan, Oleksii Kuchaiev, Patrick LeGresley, Hui Li, Jiwei Liu, Zihan Liu, Eileen Long, Ameya Sunil Mahabaleshwarkar, Somshubra Majumdar, James Maki, Miguel Martinez, Maer Rodrigues de Melo, Ivan Moshkov, Deepak Narayanan, Sean Narenthiran, Jesus Navarro, Phong Nguyen, Osvald Nitski, Vahid Noroozi, Guruprasad Nutheti, Christopher Parisien, Jupinder Parmar, Mostofa Patwary, Krzysztof Pawelec, Wei Ping, Shrimai Prabhumoye, Rajarshi Roy, Trisha Saar, Vasanth Rao Naik Sabavat, Sanjeev Satheesh, Jane Polak Scowcroft, Jason Sewall, Pavel Shamis, Gerald Shen, Mohammad Shoeybi, Dave Sizer, Misha Smelyanskiy, Felipe Soares, Makesh Narsimhan Sreedhar, Dan Su, Sandeep Subramanian, Shengyang Sun, Shubham Toshniwal, Hao Wang, Zhilin Wang, Jiaxuan You, Jiaqi Zeng, Jimmy Zhang, Jing Zhang, Vivienne Zhang, Yian Zhang, Chen Zhu)

> We release the Nemotron-4 340B model family, including Nemotron-4-340B-Base, Nemotron-4-340B-Instruct, and Nemotron-4-340B-Reward. Our models are open access under the NVIDIA Open Model License Agreement, a permissive model license that allows distribution, modification, and use of the models and its outputs. These models perform competitively to open access models on a wide range of evaluation benchmarks, and were sized to fit on a single DGX H100 with 8 GPUs when deployed in FP8 precision. We believe that the community can benefit from these models in various research studies and commercial applications, especially for generating synthetic data to train smaller language models. Notably, over 98% of data used in our model alignment process is synthetically generated, showcasing the effectiveness of these models in generating synthetic data. To further support open research and facilitate model development, we are also open-sourcing the synthetic data generation pipeline used in our model alignment process.

Nemotron-4 340B 테크니컬 리포트. 많은 사람들이 열광하긴 하던데 저는 340B, 9T 학습이라는 스펙에 부합하는 성능이 맞을까 하는 생각은 있습니다. Nemotron-4 15B (https://arxiv.org/abs/2402.16819) 또한 15B/8T 학습 모델의 성능이 7B 모델들과 비슷하다는 점에서 LLM을 학습하는 레시피 중 놓치고 있는 부분이 있다고 생각하게된 계기 중 하나였습니다. 340B 모델도 좀 비슷한 느낌이 있네요.

정렬 데이터로는 꾸준히 구축해온 HelpSteer2 데이터셋 (https://arxiv.org/abs/2406.08673) 을 사용했네요. 10K 규모의 Preference 데이터인데 어노테이터를 동원해 직접 구축한 데이터라 흥미로운 디테일들이 있습니다.

여기서 흥미로운 것 중 하나는 하나의 샘플을 최소 3명의 어노테이터가 어노테이션 했다는 점입니다. Disagreement가 높은 경우 두 명의 어노테이터를 더 참여시키는 프로세스입니다. Anthropic에서 Harmlessness 평가 데이터셋을 구축하면서 4명의 어노테이터의 합의를 통해 레이블링을 했다고 하는데 (https://arxiv.org/abs/2310.13798) 어쩌면 이런 형태의 어노테이션이 현재 표준일 수 있겠다는 생각이 드네요.

다만 이렇게 구축한 데이터의 양이 많지 않아서 생성 데이터를 많이 사용했습니다. 주로 Mistral-8x7B Instruct와 Nemotron 자체를 사용해서 프롬프트를 생성하고 Preference를 구축했네요. Mistral 모델에 대한 의존성도 없으면 최선이긴 하겠지만 그래도 Permissive License 내에서 해결하려 했다는 점이 좋은 점이 아닐까 싶습니다.

#llm #alignment

# Links

[[231020 Specific versus General Principles for Constitutional AI.md]]
[[240612 HelpSteer2.md]]
[[240226 Nemotron-4 15B Technical Report.md]]