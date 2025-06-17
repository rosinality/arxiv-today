https://arxiv.org/abs/2410.17215

*MiniPLM: Knowledge Distillation for Pre-Training Language Models* (Yuxian Gu, Hao Zhou, Fandong Meng, Jie Zhou, Minlie Huang)

> Knowledge distillation (KD) is widely used to train small, high-performing student language models (LMs) using large teacher LMs. While effective in fine-tuning, KD during pre-training faces challenges in efficiency, flexibility, and effectiveness. Existing methods either incur high computational costs due to online teacher inference, require tokenization matching between teacher and student LMs, or risk losing the difficulty and diversity of the teacher-generated training data. To address these issues, we propose MiniPLM, a KD framework for pre-training LMs by refining the training data distribution with the teacher's knowledge. For efficiency, MiniPLM performs offline teacher LM inference, allowing KD for multiple student LMs without adding training-time costs. For flexibility, MiniPLM operates solely on the training corpus, enabling KD across model families. For effectiveness, MiniPLM leverages the differences between large and small LMs to enhance the difficulty and diversity of the training data, helping student LMs acquire versatile and sophisticated knowledge. Extensive experiments demonstrate that MiniPLM boosts the student LMs' performance on 9 widely used downstream tasks, improves the language modeling capabilities, and reduces pre-training computation. The benefit of MiniPLM extends to large pre-training scales, evidenced by the extrapolation of the scaling curves. Further analysis reveals that MiniPLM supports KD across model families and enhances the utilization of pre-training data. Our model, code, and data are available at https://github.com/thu-coai/MiniPLM.

LM에 대한 Knowledge Distillation 방법. Knowledge Distillation을 좀 더 쉽게 하려는 접근인데 결과적으로는 Teacher 모델과 레퍼런스 모델의 차이가 큰 샘플들을 샘플링하는 방법이군요. Learnability와 비슷한 접근 같네요. (https://arxiv.org/abs/2206.07137)

<english>
Knowledge distillation method for LM. It tries to simplify knowledge distillation, and the resulting technique is that sampling the data which has larger difference between teacher and reference models. I think it is similar approach to learnability. (https://arxiv.org/abs/2206.07137)
</english>

#distillation

# Links

