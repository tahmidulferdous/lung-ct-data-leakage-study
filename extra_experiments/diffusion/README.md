# Class-conditional DDPM for CT slice augmentation

Work beyond the thesis. A denoising diffusion model trained on the same dataset for the same augmentation purpose, run before the rectified-flow attempt.
![Uploading image.png…]()

| | |
| --- | --- |
| Runs | 5 |
| Period | 2026-02-22 to 2026-02-22 |
| Logged compute | 4.2 GPU-hours |
| Hardware | free-tier Kaggle, Tesla T4 or TPU v3-8 |
| Tracking | [Weights & Biases](https://wandb.ai/tahmidulkashfi15-international-islamic-university-chittagong/ct-diffusion-augmentation) |

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
| ddpm-2xT4-ddp | 2026-02-22 | 7 min |
| ddpm-2xT4-ddp | 2026-02-22 | 5 min |
| ddpm-2xT4-ddp | 2026-02-22 | 80 min |
| ddpm-2xT4-ddp | 2026-02-22 | 12 min |
| ddpm-2xT4-ddp | 2026-02-22 | 147 min |

Part of [lung-ct-data-leakage-study](../..). Original Weights & Biases project name: `ct-diffusion-augmentation`.
