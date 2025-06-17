https://pytorch.org/blog/flexattention/

*FlexAttention: The Flexibility of PyTorch with the Performance of FlashAttention* (Team PyTorch)

이야기가 나오던 FlexAttention이 등장했네요. Attention Score를 변형하거나 Masking 할 수 있는 방법을 제공하는 것으로 수많은 Attention의 변형을 지원할 수 있고, 이를 torch.compile로 결합해 효율적인 Attention 구현으로 만들어낼 수 있다는 것입니다.

이전에 까다로웠던 Attention 패턴들, Prefix LM이나 Document Masking 등을 모두 간단하게 지원할 수 있네요. Flash Attention에서 지원이 되어야 한다는 제약이 사라졌으니 이제 훨씬 다양한 시도들을 해볼 수 있게 되지 않을까 싶습니다.

#efficiency 