https://arxiv.org/abs/2503.14489

*Stable Virtual Camera: Generative View Synthesis with Diffusion Models* (Jensen (Jinghao)Zhou, Hang Gao, Vikram Voleti, Aaryaman Vasishta, Chun-Han Yao, Mark Boss, Philip Torr, Christian Rupprecht, Varun Jampani)

> We present Stable Virtual Camera (Seva), a generalist diffusion model that creates novel views of a scene, given any number of input views and target cameras. Existing works struggle to generate either large viewpoint changes or temporally smooth samples, while relying on specific task configurations. Our approach overcomes these limitations through simple model design, optimized training recipe, and flexible sampling strategy that generalize across view synthesis tasks at test time. As a result, our samples maintain high consistency without requiring additional 3D representation-based distillation, thus streamlining view synthesis in the wild. Furthermore, we show that our method can generate high-quality videos lasting up to half a minute with seamless loop closure. Extensive benchmarking demonstrates that Seva outperforms existing methods across different datasets and settings.

Diffusion 기반 Novel View Synthesis. M개 이미지와 카메라 포즈 정보를 통해 N개 이미지를 생성하는 방식이군요. 샘플링 과정에서 3D Consistency가 문제인데 앵커 프레임을 경유하는 방법을 사용했습니다.

<english>
Novel view synthesis based on diffusion. It is method of generating N imgaes from M images and camera poses. Ensuring 3D consistency during sampling is main problem, and this work resolves it by using anchor frames and generate images via it.
</english>

#diffusion #novel-view-synthesis 