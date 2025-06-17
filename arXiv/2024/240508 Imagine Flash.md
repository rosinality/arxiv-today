https://arxiv.org/abs/2405.05224

*Imagine Flash: Accelerating Emu Diffusion Models with Backward Distillation* (Jonas Kohler, Albert Pumarola, Edgar Schönfeld, Artsiom Sanakoyeu, Roshan Sumbaly, Peter Vajda, Ali Thabet)

> Diffusion models are a powerful generative framework, but come with expensive inference. Existing acceleration methods often compromise image quality or fail under complex conditioning when operating in an extremely low-step regime. In this work, we propose a novel distillation framework tailored to enable high-fidelity, diverse sample generation using just one to three steps. Our approach comprises three key components: (i) Backward Distillation, which mitigates training-inference discrepancies by calibrating the student on its own backward trajectory; (ii) Shifted Reconstruction Loss that dynamically adapts knowledge transfer based on the current time step; and (iii) Noise Correction, an inference-time technique that enhances sample quality by addressing singularities in noise prediction. Through extensive experiments, we demonstrate that our method outperforms existing competitors in quantitative metrics and human evaluations. Remarkably, it achieves performance comparable to the teacher model using only three denoising steps, enabling efficient high-quality generation.

Emu (https://arxiv.org/abs/2309.15807) 에 대한 Distillation. 이전에도 지적되었던 학습과 샘플링 사이의 갭 문제에 대해서 태클하고 있네요. (https://arxiv.org/abs/2305.08891, https://arxiv.org/abs/2312.00210) 기본적으로 Student 모델이 디노이징한 결과를 Teacher 모델이 디노이징해서 타겟으로 사용하는 방식입니다. 추가적으로 Student 모델이 디노이징한 결과에 대해서 다시 노이즈를 걸어 Distillation 과정에서 중점적으로 학습할 시점을 옮길 수 있도록 했네요.

#efficiency #diffusion #distillation

# Links

[[230515 Common Diffusion Noise Schedules and Sample Steps are Flawed.md]]
[[231130 DREAM.md]]