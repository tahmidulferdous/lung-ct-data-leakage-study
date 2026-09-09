# Concatenated CNN and attention model, both split conditions

A from-scratch reimplementation of the dual-branch CNN with two four-head attention blocks from the base paper, about 666K parameters, with CLAHE preprocessing.

| | |
| --- | --- |
| Runs | 31 |
| Period | 2026-04-25 to 2026-06-24 |
| Logged compute | 11.4 GPU-hours |
| Hardware | free-tier Kaggle, Tesla T4 or TPU v3-8 |
| Tracking | [Weights & Biases](https://wandb.ai/tahmidulkashfi15-international-islamic-university-chittagong/ccal_paper_reproduction) |

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
| ccal_paper_method_leaky_split | 2026-04-25 | - | 7 min |
| ccal_paper_method_leaky_split | 2026-04-25 | - | 49 min |
| ccal_paper_method_leaky_split | 2026-04-25 | - | 0 min |
| ccal_paper_method_leaky_split | 2026-04-25 | - | 0 min |
| ccal_paper_method_leaky_split | 2026-04-25 | - | 1 min |
| ccal_paper_method_leaky_split | 2026-04-25 | - | 11 min |
| ccal_paper_method_leaky_split | 2026-04-25 | - | 30 min |
| ccal_paper_method_leaky_split | 2026-04-25 | - | 2 min |
| ccal_paper_method_leaky_split | 2026-04-25 | - | 8 min |
| ccal_paper_method_leaky_split | 2026-04-25 | - | 10 min |
| ccal_paper_method_leaky_split | 2026-04-25 | - | 4 min |
| ccal_paper_method_leaky_split | 2026-04-25 | - | 2 min |
| ccal_paper_method_leaky_split | 2026-04-25 | 99.55 | 41 min |
| ccal_paper_method_leaky_split | 2026-04-25 | 87.27 | 38 min |
| ccal_sequential_split_no_shuffle | 2026-04-26 | 87.5 | 39 min |
| ccal_paper_method_leaky_split | 2026-04-26 | 98.64 | 38 min |
| ccal_paper_method_leaky_split | 2026-04-26 | 97.73 | 39 min |
| ccal_paper_method_leaky_split | 2026-04-26 | - | 0 min |
| ccal_paper_method_leaky_split | 2026-04-26 | - | 37 min |
| ccal_sequential_split_no_shuffle | 2026-04-26 | 83.93 | 38 min |
| ccal_sequential_split_no_shuffle | 2026-04-26 | 85.71 | 38 min |
| ccal_sequential_split_no_shuffle | 2026-06-23 | - | 0 min |
| ccal_sequential_split_no_shuffle | 2026-06-23 | 96.38 | 29 min |
| ccal_sequential_split_no_shuffle | 2026-06-23 | 98.19 | 29 min |
| ccal_sequential_split_no_shuffle | 2026-06-23 | 95.93 | 28 min |
| ccal_sequential_split_no_shuffle | 2026-06-23 | 87.33 | 29 min |
| ccal_sequential_split_no_shuffle | 2026-06-23 | 88.69 | 28 min |
| ccal_sequential_split_no_shuffle | 2026-06-23 | 88.24 | 28 min |
| ccal_sequential_split_no_shuffle | 2026-06-24 | 87.78 | 26 min |
| ccal_sequential_split_no_shuffle | 2026-06-24 | 90.95 | 27 min |
| ccal_sequential_split_no_shuffle | 2026-06-24 | 88.69 | 27 min |

Part of [lung-ct-data-leakage-study](../..). Original Weights & Biases project name: `ccal_paper_reproduction`.
