# The controlled measurement: same model, same ratio, same seeds, split changed

This is the headline experiment. One architecture, one 70/20/10 ratio and three seeds, trained twice, changing only whether the slice list is shuffled before it is cut. Everything else in this repository leads here.

| | |
| --- | --- |
| Runs | 6 |
| Period | 2026-06-24 to 2026-06-24 |
| Logged compute | 2.7 GPU-hours |
| Hardware | free-tier Kaggle, Tesla T4 or TPU v3-8 |
| Tracking | [Weights & Biases](https://wandb.ai/tahmidulkashfi15-international-islamic-university-chittagong/lung-base-bench) |

## What is here

| Path | Contents |
| --- | --- |
| `runs.csv` | one row per run, every hyperparameter and every logged metric |
| `figures/` | evaluation figures, grouped by run |
| `code/` | the training code as it ran on Kaggle |
| `weights/` | the final checkpoint |

## Runs

| Run | Date | test/accuracy | Runtime |
| --- | --- | --- | --- |
| ccal_shuffled_0.70-0.20-0.10_seed42 | 2026-06-24 | 95.5 | 27 min |
| ccal_shuffled_0.70-0.20-0.10_seed123 | 2026-06-24 | 97.3 | 27 min |
| ccal_shuffled_0.70-0.20-0.10_seed2024 | 2026-06-24 | 94.59 | 27 min |
| ccal_sorted_0.70-0.20-0.10_seed42 | 2026-06-24 | 86.49 | 27 min |
| ccal_sorted_0.70-0.20-0.10_seed123 | 2026-06-24 | 87.39 | 27 min |
| ccal_sorted_0.70-0.20-0.10_seed2024 | 2026-06-24 | 90.99 | 27 min |

Part of [lung-ct-data-leakage-study](../..). Original Weights & Biases project name: `lung-base-bench`.
