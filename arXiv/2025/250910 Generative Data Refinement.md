https://arxiv.org/abs/2509.08653

*Generative Data Refinement: Just Ask for Better Data* (Minqi Jiang, João G. M. Araújo, Will Ellsworth, Sian Gooding, Edward Grefenstette)

> For a fixed parameter size, the capabilities of large models are primarily determined by the quality and quantity of its training data. Consequently, training datasets now grow faster than the rate at which new data is indexed on the web, leading to projected data exhaustion over the next decade. Much more data exists as user-generated content that is not publicly indexed, but incorporating such data comes with considerable risks, such as leaking private information and other undesirable content. We introduce a framework, Generative Data Refinement (GDR), for using pretrained generative models to transform a dataset with undesirable content into a refined dataset that is more suitable for training. Our experiments show that GDR can outperform industry-grade solutions for dataset anonymization, as well as enable direct detoxification of highly unsafe datasets. Moreover, we show that by generating synthetic data that is conditioned on each example in the real dataset, GDR's refined outputs naturally match the diversity of web scale datasets, and thereby avoid the often challenging task of generating diverse synthetic data via model prompting. The simplicity and effectiveness of GDR make it a powerful tool for scaling up the total stock of training data for frontier models.

LLM을 사용한 웹 코퍼스의 익명화와 독성 제거.

Anonymization and detoxification of web corpus using LLMs.

#pretraining #corpus #synthetic-data 