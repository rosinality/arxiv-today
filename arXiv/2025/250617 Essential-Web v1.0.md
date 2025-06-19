https://arxiv.org/abs/2506.14111

*Essential-Web v1.0: 24T tokens of organized web data* (Essential AI: Andrew Hojel, Michael Pust, Tim Romanski, Yash Vanjani, Ritvik Kapila, Mohit Parmar, Adarsh Chaluvaraju, Alok Tripathy, Anil Thomas, Ashish Tanwer, Darsh J Shah, Ishaan Shah, Karl Stratos, Khoi Nguyen, Kurt Smith, Michael Callahan, Peter Rushton, Philip Monk, Platon Mazarakis, Saad Jamal, Saurabh Srivastava, Somanshu Singla, Ashish Vaswani)

> Data plays the most prominent role in how language models acquire skills and knowledge. The lack of massive, well-organized pre-training datasets results in costly and inaccessible data pipelines. We present Essential-Web v1.0, a 24-trillion-token dataset in which every document is annotated with a twelve-category taxonomy covering topic, format, content complexity, and quality. Taxonomy labels are produced by EAI-Distill-0.5b, a fine-tuned 0.5b-parameter model that achieves an annotator agreement within 3% of Qwen2.5-32B-Instruct. With nothing more than SQL-style filters, we obtain competitive web-curated datasets in math (-8.0% relative to SOTA), web code (+14.3%), STEM (+24.5%) and medical (+8.6%). Essential-Web v1.0 is available on HuggingFace: https://huggingface.co/datasets/EssentialAI/essential-web-v1.0

Common Crawl에서 추출한 24B 문서, 24T 토큰에 대해 카테고리를 부여해 큐레이션했네요. 요즘 대세인 LLM 기반 전처리에 대한 상세한 리포트군요.

<english>
The study that curated 24B documents, 24T tokens extracted from Common Crawl by assigning categories. It is a detailed report on LLM based preprocessing which is currently mainstream.
</english>

#pretraining #corpus 