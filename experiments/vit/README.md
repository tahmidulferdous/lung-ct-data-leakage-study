# ViT-B/16, both split conditions

An 85.8M-parameter vision transformer, the high-capacity end of the comparison.

| | |
| --- | --- |
| Runs | 2 |
| Period | 2026-04-27 to 2026-04-27 |
| Logged compute | 3.4 GPU-hours |
| Hardware | free-tier Kaggle, Tesla T4 or TPU v3-8 |
| Tracking | [Weights & Biases](https://wandb.ai/tahmidulkashfi15-international-islamic-university-chittagong/vit_lung_reproduction) |

## What is here

| Path | Contents |
| --- | --- |
| `runs.csv` | one row per run, every hyperparameter and every logged metric |
| `figures/` | evaluation figures, grouped by run |
| `code/` | the training code as it ran on Kaggle |
| | *No checkpoint was uploaded for these runs. The code and the logged metrics are the record.* |

## Runs

| Run | Date | best_val_acc | Runtime |
| --- | --- | --- | --- |
| vit_leaky_split | 2026-04-27 | 96.59 | 156 min |
| vit_sequential_split | 2026-04-27 | 72.48 | 48 min |

Part of [lung-ct-data-leakage-study](../..). Original Weights & Biases project name: `vit_lung_reproduction`.
