# A published four-block CNN, both split conditions

The roughly 2M-parameter four-block CNN from the PLOS ONE paper, retrained to check the effect is not specific to one architecture.

| | |
| --- | --- |
| Runs | 2 |
| Period | 2026-04-27 to 2026-04-28 |
| Logged compute | 0.2 GPU-hours |
| Hardware | free-tier Kaggle, Tesla T4 or TPU v3-8 |
| Tracking | [Weights & Biases](https://wandb.ai/tahmidulkashfi15-international-islamic-university-chittagong/plos_one_lung_reproduction) |

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
| plos_cnn_leaky_split | 2026-04-27 | 90.91 | 7 min |
| plos_cnn_sequential_split | 2026-04-28 | 83.94 | 5 min |

Part of [lung-ct-data-leakage-study](../..). Original Weights & Biases project name: `plos_one_lung_reproduction`.
