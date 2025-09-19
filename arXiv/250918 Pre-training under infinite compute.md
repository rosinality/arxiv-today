https://arxiv.org/abs/2509.14786

*Pre-training under infinite compute* (Konwoo Kim, Suhas Kotha, Percy Liang, Tatsunori Hashimoto)

> Since compute grows much faster than web text available for language model pre-training, we ask how one should approach pre-training under fixed data and no compute constraints. We first show that existing data-constrained approaches of increasing epoch count and parameter count eventually overfit, and we significantly improve upon such recipes by properly tuning regularization, finding that the optimal weight decay is $30\times$ larger than standard practice. Since our regularized recipe monotonically decreases loss following a simple power law in parameter count, we estimate its best possible performance via the asymptote of its scaling law rather than the performance at a fixed compute budget. We then identify that ensembling independently trained models achieves a significantly lower loss asymptote than the regularized recipe. Our best intervention combining epoching, regularization, parameter scaling, and ensemble scaling achieves an asymptote at 200M tokens using $5.17\times$ less data than our baseline, and our data scaling laws predict that this improvement persists at higher token budgets. We find that our data efficiency gains can be realized at much smaller parameter counts as we can distill an ensemble into a student model that is 8$\times$ smaller and retains $83\%$ of the ensembling benefit. Finally, our interventions designed for validation loss generalize to downstream benchmarks, achieving a $9\%$ improvement for pre-training evals and a $17.5\times$ data efficiency improvement over continued pre-training on math mid-training data. Our results show that simple algorithmic improvements can enable significantly more data-efficient pre-training in a compute-rich future.

(필요하다면 3.0보다 큰) Weight decay와 Epoch 수를 튜닝하는 것으로 연산을 쓰고 싶은 만큼 투입할 수 있다는 연구. 파라미터를 키우거나 앙상블을 할 수 있음. 최적 Weight decay와 Epoch 수를 어떻게 찾을 수 있는가 하는 것은 문제.

<english>
Tuning weight decay (it could be > 3.0) and epoch count allows you to use as much compute as you want (in the form of parameters or ensembles). Whether it would be possible to find the optimal weight decay and epoch count would be a problem.
</english>

#scaling-law #pretraining 