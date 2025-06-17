https://arxiv.org/abs/2407.07860

*Controlling Space and Time with Diffusion Models* (Daniel Watson, Saurabh Saxena, Lala Li, Andrea Tagliasacchi, David J. Fleet)

> We present 4DiM, a cascaded diffusion model for 4D novel view synthesis (NVS), conditioned on one or more images of a general scene, and a set of camera poses and timestamps. To overcome challenges due to limited availability of 4D training data, we advocate joint training on 3D (with camera pose), 4D (pose+time) and video (time but no pose) data and propose a new architecture that enables the same. We further advocate the calibration of SfM posed data using monocular metric depth estimators for metric scale camera control. For model evaluation, we introduce new metrics to enrich and overcome shortcomings of current evaluation schemes, demonstrating state-of-the-art results in both fidelity and pose control compared to existing diffusion models for 3D NVS, while at the same time adding the ability to handle temporal dynamics. 4DiM is also used for improved panorama stitching, pose-conditioned video to video translation, and several other tasks. For an overview see https://4d-diffusion.github.io

https://4d-diffusion.github.io/

Few-shot Novel View Synthesis + Time. 사실 이제 이런 모델들에서는 Neural Rendering스러운 점은 거의 없네요. 카메라 포즈와 시간 정보를 조건으로 주고 카메라 포즈 없는 비디오 데이터도 같이 학습했군요. Sora에서 나타난 강력한 3D Consistency를 생각하면 이 문제에 대해 비디오가 할 수 있는 역할이 많은 것 같습니다.

#neural-rendering #diffusion 