https://github.com/deepseek-ai/DeepGEMM

*DeepGEMM* (Chenggang Zhao and Liang Zhao and Jiashi Li and Zhean Xu)

> 

DeepSeek이 오늘 공개한 건 FP8 GEMM 커널이군요. 논문에 언급됐던 Fine-grained Quantization과 고정밀도 Accumulation이 구현된 GEMM, 그리고 MoE를 위한 Grouped GEMM 커널입니다. 컴파일된 바이너리를 뜯어고치는 묘기까지 했네요.

<english>
Today's opensource release from DeepSeek is FP8 GEMM kernel. It includes GEMM and Grouped GEMM kernel for MoE that implements fine-grained quantization and high precision accumulation mentioned in the paper. They even patched compiled binary for efficiency.
</english>

#efficiency 