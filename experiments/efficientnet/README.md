# EfficientNet B0 through B4, both split conditions

ImageNet-pretrained EfficientNet backbones from B0 to B4, 4M to 17.6M parameters, with lung-contour cropping, so the leakage gap can be read across model capacity.

| | |
| --- | --- |
| Runs | 16 |
| Period | 2026-04-27 to 2026-06-25 |
| Logged compute | 11.2 GPU-hours |
| Hardware | free-tier Kaggle, Tesla T4 or TPU v3-8 |
| Tracking | [Weights & Biases](https://wandb.ai/tahmidulkashfi15-international-islamic-university-chittagong/lung_effnet_reproduction) |

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
| lung_effnet_leaky_split | 2026-04-27 | 100 | 35 min |
| lung_effnet_leaky_split | 2026-04-27 | - | 3 min |
| lung_effnet_leaky_split | 2026-04-27 | 98.86 | 36 min |
| lung_effnet_sequential_split | 2026-04-27 | 90.37 | 33 min |
| lung_effnet_sequential_split | 2026-06-23 | 93.67 | 48 min |
| lung_effnet_sequential_split | 2026-06-23 | 91.86 | 50 min |
| lung_effnet_sequential_split | 2026-06-23 | 90.95 | 51 min |
| lung_effnet_sequential_split | 2026-06-23 | 93.67 | 47 min |
| lung_effnet_sequential_split | 2026-06-23 | 91.86 | 50 min |
| lung_effnet_sequential_split | 2026-06-23 | 90.95 | 53 min |
| effnet_shuffled_seed42 | 2026-06-25 | 98.64 | 43 min |
| effnet_shuffled_seed123 | 2026-06-25 | 99.55 | 44 min |
| effnet_shuffled_seed2024 | 2026-06-25 | 99.55 | 52 min |
| effnet_sorted_seed42 | 2026-06-25 | 90.5 | 31 min |
| effnet_sorted_seed123 | 2026-06-25 | 92.31 | 48 min |
| effnet_sorted_seed2024 | 2026-06-25 | 92.31 | 49 min |

Part of [lung-ct-data-leakage-study](../..). Original Weights & Biases project name: `lung_effnet_reproduction`.
