https://arxiv.org/abs/2311.09431

Striped Attention: Faster Ring Attention for Causal Transformers (William Brandon, Aniruddha Nrusimha, Kevin Qian, Zachary Ankner, Tian Jin, Zhiye Song, Jonathan Ragan-Kelley)

Ring Attention (https://arxiv.org/abs/2310.01889) 에 대한 개선 작업이군요. Ring Attention에서는 Key/Value를 연속된 형태로 자르는데, Causal Mask를 생각하면 계산이 필요하지 않은 블럭들이 있죠. 그런데 이 블럭들이 워커마다 불균일하게 발생하기 때문에 (어떤 워커에서는 계산이 필요한데 다른 워커에서는 계산이 필요한 등) 이 문제를 해소하기 위해 연속된 형태가 아니라 일정 스텝만큼 건너뛰는 형태로 잘라서 계산한다는 아이디어입니다.

#efficient_training

# Links

[[231003 Ring Attention with Blockwise Transformers for Near-Infinite Context.md]]