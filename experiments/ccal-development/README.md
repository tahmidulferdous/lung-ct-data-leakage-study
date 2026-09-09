# Ninety runs of architecture search behind the reimplementation

The development history that produced the configuration used above. Kept because the search is the evidence of how that configuration was arrived at, not guessed.

| | |
| --- | --- |
| Runs | 90 |
| Period | 2025-09-24 to 2025-10-31 |
| Logged compute | 5.4 GPU-hours |
| Hardware | free-tier Kaggle, Tesla T4 or TPU v3-8 |
| Tracking | [Weights & Biases](https://wandb.ai/tahmidulkashfi15-international-islamic-university-chittagong/base_ccal) |

## What is here

| Path | Contents |
| --- | --- |
| `runs.csv` | one row per run, every hyperparameter and every logged metric |
| `figures/` | evaluation figures, grouped by run |
| `code/` | the training code as it ran on Kaggle |
| `weights/` | the final checkpoint |

## Runs

| Run | Date | test_accuracy | Runtime |
| --- | --- | --- | --- |
| base_model_training_CLAHE_OFF | 2025-09-24 | 84.55 | 8 min |
| base_model_training_CLAHE_ON | 2025-09-24 | 65 | 9 min |
| base_model_training | 2025-09-25 | 52.27 | 7 min |
| base_model_training | 2025-09-25 | 92.73 | 7 min |
| base_model_training | 2025-09-25 | 51.36 | 7 min |
| base_model_training | 2025-09-25 | 39.09 | 8 min |
| base_model_training | 2025-09-25 | - | 4 min |
| base_model_training | 2025-09-25 | - | 1 min |
| base_model_training | 2025-09-25 | 11.82 | 7 min |
| base_model_training | 2025-09-25 | - | 18 min |
| base_model_training | 2025-09-25 | - | 1 min |
| base_model_training | 2025-09-25 | - | 3 min |
| base_model_training | 2025-09-26 | 88.64 | 3 min |
| base_model_training | 2025-09-26 | - | 0 min |
| base_model_training | 2025-09-26 | 88.64 | 3 min |
| base_model_training | 2025-09-26 | - | 5 min |
| base_model_training | 2025-09-26 | - | 1 min |
| base_model_training | 2025-09-26 | 51.82 | 3 min |
| base_model_training | 2025-09-26 | 100 | 3 min |
| base_model_training | 2025-09-26 | - | 2 min |
| base_model_training | 2025-09-27 | 98.18 | 4 min |
| base_model_training | 2025-09-27 | 98.18 | 4 min |
| base_model_training | 2025-09-27 | 95 | 4 min |
| base_model_training | 2025-09-27 | 77.73 | 3 min |
| base_model_training | 2025-09-27 | - | 1 min |
| base_model_training | 2025-09-27 | - | 1 min |
| base_model_training | 2025-09-27 | 99.55 | 4 min |
| base_model_training | 2025-09-27 | 98.18 | 4 min |
| base_model_training | 2025-09-27 | - | 0 min |
| base_model_training | 2025-09-27 | - | 1 min |
| base_model_training | 2025-09-27 | 98.64 | 3 min |
| base_model_training | 2025-09-27 | - | 1 min |
| base_model_training | 2025-09-27 | - | 0 min |
| base_model_training | 2025-09-27 | - | 1 min |
| base_model_training | 2025-09-27 | 99.09 | 3 min |
| base_model_training | 2025-09-28 | - | 0 min |
| base_model_training | 2025-09-28 | - | 0 min |
| base_model_training | 2025-09-28 | 45.91 | 9 min |
| base_model_training | 2025-09-28 | 82.73 | 5 min |
| base_model_training | 2025-09-28 | - | 2 min |
| base_model_training | 2025-09-28 | - | 0 min |
| base_model_training | 2025-09-28 | - | 2 min |
| base_model_training | 2025-09-28 | - | 4 min |
| base_model_training | 2025-09-28 | 78.64 | 5 min |
| base_model_training | 2025-09-28 | 99.55 | 4 min |
| base_model_training | 2025-09-28 | - | 0 min |
| base_model_training | 2025-09-28 | 82.27 | 4 min |
| base_model_training | 2025-09-28 | 88.18 | 9 min |
| base_model_training | 2025-09-28 | - | 4 min |
| base_model_training | 2025-09-28 | - | 5 min |
| base_model_training | 2025-09-28 | 86.36 | 7 min |
| base_model_training | 2025-09-29 | - | 14 min |
| base_model_training | 2025-09-29 | - | 3 min |
| base_model_training | 2025-09-29 | - | 3 min |
| base_model_training | 2025-09-29 | - | 2 min |
| base_model_training | 2025-09-29 | 37.73 | 7 min |
| base_model_training | 2025-09-29 | 84.55 | 7 min |
| base_model_training | 2025-09-30 | - | 5 min |
| base_model_training | 2025-09-30 | 77.73 | 10 min |
| base_model_training | 2025-09-30 | - | 0 min |
| base_model_training | 2025-09-30 | - | 0 min |
| base_model_training | 2025-09-30 | - | 0 min |
| base_model_training | 2025-09-30 | - | 0 min |
| base_model_training | 2025-09-30 | - | 0 min |
| base_model_training | 2025-09-30 | - | 1 min |
| base_model_training | 2025-09-30 | - | 1 min |
| base_model_training | 2025-09-30 | - | 0 min |
| base_model_training | 2025-09-30 | - | 0 min |
| base_model_training | 2025-09-30 | - | 0 min |
| base_model_training | 2025-09-30 | - | 1 min |
| base_model_training | 2025-09-30 | 42.73 | 4 min |
| base_model_training | 2025-09-30 | 55 | 4 min |
| base_model_training | 2025-09-30 | 60 | 4 min |
| base_model_training | 2025-09-30 | 71.82 | 4 min |
| base_model_training | 2025-10-04 | 100 | 4 min |
| base_model_training | 2025-10-04 | 99.45 | 6 min |
| base_model_training | 2025-10-04 | 87.97 | 6 min |
| base_model_training | 2025-10-04 | - | 1 min |
| base_model_training | 2025-10-04 | - | 0 min |
| base_model_training | 2025-10-04 | 79.55 | 4 min |
| base_model_training | 2025-10-04 | 86.82 | 4 min |
| base_model_training | 2025-10-04 | - | 1 min |
| base_model_training | 2025-10-04 | - | 3 min |
| base_model_training | 2025-10-16 | - | 0 min |
| base_model_training | 2025-10-16 | - | 0 min |
| base_model_training | 2025-10-31 | 85 | 7 min |
| base_model_training | 2025-10-31 | 85 | 7 min |
| base_model_training | 2025-10-31 | - | 2 min |
| base_model_training | 2025-10-31 | 85.91 | 6 min |
| base_model_training | 2025-10-31 | 79.09 | 13 min |

Part of [lung-ct-data-leakage-study](../..). Original Weights & Biases project name: `base_ccal`.
