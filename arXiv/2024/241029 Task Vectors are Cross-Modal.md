https://arxiv.org/abs/2410.22330

*Task Vectors are Cross-Modal* (Grace Luo, Trevor Darrell, Amir Bar)

> We investigate the internal representations of vision-and-language models (VLMs) and how they encode task representations. We consider tasks specified through examples or instructions, using either text or image inputs. Surprisingly, we find that conceptually similar tasks are mapped to similar task vector representations, regardless of how they are specified. Our findings suggest that to output answers, tokens in VLMs undergo three distinct phases: input, task, and answer, a process which is consistent across different modalities and specifications. The task vectors we identify in VLMs are general enough to be derived in one modality (e.g., text) and transferred to another (e.g., image). Additionally, we find that ensembling exemplar and instruction based task vectors produce better task representations. Taken together, these insights shed light on the underlying mechanisms of VLMs, particularly their ability to represent tasks in a shared manner across different modalities and task specifications. Project page: https://task-vectors-are-cross-modal.github.io.

In-context Learning 프롬프트에서 추출한 과제의 내용을 기술하는 임베딩이 모달리티 사이에 공통적으로 작동한다는 연구. 즉 텍스트로 작성한 과제에 대한 임베딩을 이미지 입력에 대해 사용하면 이미지에 대해 동일한 과제를 수행한다고 합니다. 이미지와 텍스트의 정렬이 이미지-텍스트 모델의 성능에 중요하다는 것과 관련이 있지 않을까요. (https://arxiv.org/abs/2408.16357)

<english>
Embeddings that contains information on tasks, which is extracted from in-context learning prompts, works between different modalities. That is, if you extract embeddings from tasks described in texts and use it for image inputs then model do the same tasks on images. I think it may related to results which says alignment between image and text is crucial for performance of image-text models. (https://arxiv.org/abs/2408.16357)
</english>

#in-context-learning #multimodal

# Links

[[240829 Law of Vision Representation in MLLMs.md]]