# lung-ct-data-leakage-study

**What a lung CT classifier's accuracy really is, once you stop shuffling slices between train and test**

Undergraduate thesis work and everything around it: the experiments, the code as it ran, the logged metrics for every run, and the figures those runs produced. 188 training runs in total, all on free-tier Kaggle accelerators.

## The result

| Seed | Shuffled split | File-order split | Difference |
| --- | --- | --- | --- |
| 42 | 95.50 | 86.49 | -9.01 |
| 123 | 97.30 | 87.39 | -9.91 |
| 2024 | 94.59 | 90.99 | -3.60 |
| **mean** | **95.80** | **88.29** | **-7.51** |

Test accuracy, percent. Same architecture, same 70/20/10 ratio, same seeds. The only thing that changed is whether the slice list was shuffled before it was cut. Full per-run numbers are in [experiments/split-benchmark/runs.csv](experiments/split-benchmark/runs.csv).

## What is actually being compared

The IQ-OTH/NCCD dataset ships **no patient identifier**. The filenames carry a flat slice
index, not a case number, so slices belonging to one scan cannot be grouped. Every claim
in the literature about patient-level splitting on this dataset, including an earlier
write-up of this work, is therefore unsupported by the data as released.

What can be compared, and what is compared here, is a **random shuffle of slices** against
a **split that respects file order**. The second is an *ordering split*. It is not a
patient-level split and this repository does not call it one.

The distinction is the whole point. Under a random shuffle, near-identical slices from the
same scan land on both sides of the split, and the reported accuracy is inflated by that
overlap. Holding the split ratio, the architecture and the seed fixed and changing only the
shuffle costs about **7.5 percentage points** of accuracy, measured across three seeds and
two architectures.

An earlier write-up called the ordered condition patient-level and quoted a gap of 12.46
points. Both figures were wrong: the first conflated grouping with a change in split ratio,
and the second described a split the code never performed. The numbers in this repository
supersede them.

## The experiments

| Experiment | Runs | What it is |
| --- | --- | --- |
| [split-benchmark](experiments/split-benchmark/) | 6 | The controlled measurement: same model, same ratio, same seeds, split changed |
| [ccal-reproduction](experiments/ccal-reproduction/) | 31 | Concatenated CNN and attention model, both split conditions |
| [ccal-development](experiments/ccal-development/) | 90 | Ninety runs of architecture search behind the reimplementation |
| [efficientnet](experiments/efficientnet/) | 16 | EfficientNet B0 through B4, both split conditions |
| [vit](experiments/vit/) | 2 | ViT-B/16, both split conditions |
| [plos-cnn](experiments/plos-cnn/) | 2 | A published four-block CNN, both split conditions |

## Beyond the thesis

Attempts to fix the class imbalance by generating CT slices, and one architecture exploration. None of these fed into the thesis result; they are here because they were done.

| Experiment | Runs | What it is |
| --- | --- | --- |
| [rectified-flow](extra_experiments/rectified-flow/) | 18 | Rectified flow generator for CT slice augmentation |
| [diffusion](extra_experiments/diffusion/) | 5 | Class-conditional DDPM for CT slice augmentation |
| [dsmat-mamba](extra_experiments/dsmat-mamba/) | 18 | Depthwise state-space (Mamba) classifiers on lung CT |

## Layout

```
experiments/          the four architecture families and the split benchmark
extra_experiments/    generative augmentation and one architecture probe
```

Every experiment directory holds the same four things: `runs.csv`, `figures/`, `code/`, and `weights/` where a checkpoint was saved.

## Reproducing

Training ran on free-tier Kaggle accelerators, so the notebooks reference `/kaggle/input/...`
paths and will not run unmodified on a local machine. To rerun an experiment, upload its
`code/` directory as a Kaggle notebook and attach the dataset named in the header.
Each `code/requirements.txt` is the environment as captured at run time.

## Provenance

Every `runs.csv` is exported directly from the Weights & Biases API and is not edited by
hand. Figures are the ones the training runs logged, downscaled for size. Nothing here is
reconstructed after the fact.

The wider record, all 250 runs across every project plus 162 Kaggle notebooks, is at [github.com/tahmidulferdous/ml-research-log](https://github.com/tahmidulferdous/ml-research-log).

Tahmidul Bin Ferdous, Department of Computer Science and Engineering, International Islamic University Chittagong. turing.accessories@gmail.com
