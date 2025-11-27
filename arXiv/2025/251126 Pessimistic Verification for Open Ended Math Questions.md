https://arxiv.org/abs/2511.21522

*Pessimistic Verification for Open Ended Math Questions* (Yanxing Huang, Zihan Tang, Zejin Lin, Peng Li, Yang Liu)

> The key limitation of the verification performance lies in the ability of error detection. With this intuition we designed several variants of pessimistic verification, which are simple workflows that could significantly improve the verification of open-ended math questions. In pessimistic verification we construct multiple parallel verifications for the same proof, and the proof is deemed incorrect if any one of them reports an error. This simple technique significantly improves the performance across many math verification benchmarks without incurring substantial computational resources. Its token efficiency even surpassed extended long-CoT in test-time scaling. Our case studies further indicate that the majority of false negatives in stronger models are actually caused by annotation errors in the original dataset, so our method's performance is in fact underestimated. Self-verification for mathematical problems can effectively improve the reliability and performance of language model outputs, and it also plays a critical role in enabling long-horizon mathematical tasks. We believe that research on pessimistic verification will help enhance the mathematical capabilities of language models across a wide range of tasks.

증명에 대한 Pessimistic한 검증. 각 증명을 청크 단위로 여러 번 검증하고 한 번의 검증에서라도 에러가 발견되면 오류로 처리.

Pessimistic verification of proofs. Each proof is verified multiple times in a chunkwise manner, and deemed incorrect if any of the verifications finds an error.

#test-time-compute 