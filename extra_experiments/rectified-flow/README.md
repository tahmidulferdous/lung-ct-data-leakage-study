# Rectified flow generator for CT slice augmentation

Work beyond the thesis. A rectified-flow generator trained to synthesise CT slices, intended to rebalance the heavily skewed benign class. Includes a JAX/TPU implementation alongside the PyTorch one.
<img width="1100" height="287" alt="Benign" src="https://github.com/user-attachments/assets/641a4e93-8af1-45e3-9e60-770e869be47d" />


| | |
| --- | --- |
| Runs | 18 |
| Period | 2026-02-26 to 2026-03-01 |
| Logged compute | 32.1 GPU-hours |
| Hardware | free-tier Kaggle, Tesla T4 or TPU v3-8 |
| Tracking | [Weights & Biases](https://wandb.ai/tahmidulkashfi15-international-islamic-university-chittagong/ct-rectified-flow) |

## What is here

| Path | Contents |
| --- | --- |
| `runs.csv` | one row per run, every hyperparameter and every logged metric |
| `figures/` | evaluation figures, grouped by run |
| `code/` | the training code as it ran on Kaggle |
| | *No checkpoint was uploaded for these runs. The code and the logged metrics are the record.* |

## Runs

| Run | Date | Runtime |
| --- | --- | --- |
| rf-2xGPU-ddp | 2026-02-26 | 0 min |
| rf-2xGPU-ddp | 2026-02-26 | 0 min |
| rf-1xGPU | 2026-02-26 | 105 min |
| rf-2xGPU-ddp | 2026-02-26 | 276 min |
| rf-2xGPU-ddp | 2026-02-26 | 0 min |
| rf-2xGPU-ddp | 2026-02-26 | 0 min |
| rf-2xGPU-ddp | 2026-02-27 | 570 min |
| rf-2xGPU-ddp | 2026-02-27 | 407 min |
| rf-8xTPUv5e-JAX | 2026-02-27 | 34 min |
| rf-8xTPUv5e-JAX | 2026-02-27 | 40 min |
| rf-8xTPUv5e-JAX | 2026-02-27 | 62 min |
| rf-JAX-8xTPUv5e | 2026-02-27 | 133 min |
| rf-JAX-8xTPUv5e | 2026-03-01 | 72 min |
| rf-JAX-8xTPUv5e | 2026-03-01 | 60 min |
| rf-JAX-8xTPUv5e | 2026-03-01 | 12 min |
| rf-JAX-8xTPUv5e | 2026-03-01 | 0 min |
| rf-JAX-8xTPUv5e | 2026-03-01 | 129 min |
| rf-JAX-8xTPUv5e | 2026-03-01 | 26 min |
<img width="1100" height="550" alt="loss_curve" src="https://github.com/user-attachments/assets/ea5a7915-2f3a-453d-8793-a089aabfc5de" />


Part of [lung-ct-data-leakage-study](../..). Original Weights & Biases project name: `ct-rectified-flow`.
