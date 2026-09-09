# Depthwise state-space (Mamba) classifiers on lung CT

Work beyond the thesis. Depthwise separable state-space blocks as a classifier backbone on the same dataset, at Pico and Nano scales.

| | |
| --- | --- |
| Runs | 18 |
| Period | 2026-02-10 to 2026-02-11 |
| Logged compute | 1.7 GPU-hours |
| Hardware | free-tier Kaggle, Tesla T4 or TPU v3-8 |
| Tracking | [Weights & Biases](https://wandb.ai/tahmidulkashfi15-international-islamic-university-chittagong/DSMaT-LungCancer) |

## What is here

| Path | Contents |
| --- | --- |
| `runs.csv` | one row per run, every hyperparameter and every logged metric |
| `figures/` | evaluation figures, grouped by run |
| `code/` | the training code as it ran on Kaggle |
| | *No checkpoint was uploaded for these runs. The code and the logged metrics are the record.* |

## Runs

| Run | Date | val_acc | Runtime |
| --- | --- | --- | --- |
| DepthWiseMamba-Pico | 2026-02-10 | 0.8698 | 18 min |
| DepthwiseMamba-Nano | 2026-02-10 | 0.8021 | 8 min |
| DepthWiseMamba-Pico | 2026-02-10 | 0.7292 | 3 min |
| DepthWiseMamba-Pico | 2026-02-10 | - | 0 min |
| DepthWiseMamba-Pico | 2026-02-10 | - | 0 min |
| DepthWiseMamba-Pico | 2026-02-10 | 0.724 | 9 min |
| DepthWiseMamba-Pico | 2026-02-10 | - | 0 min |
| DepthWiseMamba-Pico | 2026-02-10 | 0.6823 | 24 min |
| DepthWiseMamba-Pico | 2026-02-10 | - | 0 min |
| DepthWiseMamba-Pico | 2026-02-10 | 0.875 | 16 min |
| DepthWiseMamba-Pico | 2026-02-11 | 0.8273 | 5 min |
| DepthWiseMamba-Pico | 2026-02-11 | - | 0 min |
| DepthWiseMamba-Pico | 2026-02-11 | 0.9152 | 13 min |
| DepthWiseMamba-Pico | 2026-02-11 | - | 0 min |
| DepthWiseMamba-Pico | 2026-02-11 | - | 0 min |
| DepthWiseMamba-Pico | 2026-02-11 | - | 0 min |
| DepthWiseMamba-Pico | 2026-02-11 | - | 0 min |
| DepthWiseMamba-Pico | 2026-02-11 | 0.8242 | 3 min |

Part of [lung-ct-data-leakage-study](../..). Original Weights & Biases project name: `DSMaT-LungCancer`.
