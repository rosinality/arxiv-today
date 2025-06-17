https://arxiv.org/abs/2308.13320

Fine-tuning can cripple your foundation model; preserving features may be the solution (Jishnu Mukhoti, Yarin Gal, Philip H.S. Torr, Puneet K. Dokania)

clip finetuning에서 발생하는 forgetting 문제 이야기. clip 같은 pretrained model은 unlabeled data에서 무엇을 배웠는지 알 수 없으니 무엇을 잊어버린는지 확인하는 것도 까다롭다는 이야기를 하면서 feature space가 지나치게 변화하지 않도록 penalty를 걸어주는 것으로 문제를 감소시킬 수 있다는 결과를 보여주는 군요.

#finetuning 