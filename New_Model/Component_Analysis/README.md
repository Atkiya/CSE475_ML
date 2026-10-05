## Ablation results (mean subject accuracy)

Intact cohort: 20 subjects, subject-specific models, 40 active classes, no rest class, test repetitions held out. All values are percentages. The best value in each column is in **bold**.

The numbers in brackets are the **95% bootstrap confidence interval** for the mean subject accuracy, written as [lower, upper]. The 20 subjects were resampled with replacement many times and the mean accuracy was recomputed each time. The interval is the range containing the middle 95% of those resampled means. A narrower interval means the result is more stable across subjects. If two rows' intervals overlap heavily, the difference between them is probably not significant.

| # | Ablation | Window | Whole repetition | Raw window |
|---|----------|--------|------------------|------------|
| 1 | No MLP | **98.89** [98.48, 99.23] | 99.75 [99.44, 100.00] | 98.08 [97.47, 98.61] |
| 2 | No ExtraTrees | 98.86 [98.47, 99.19] | 99.75 [99.44, 100.00] | 98.10 [97.51, 98.60] |
| 3 | No LDA | 98.55 [98.13, 98.92] | 99.56 [99.19, 99.88] | 97.62 [97.04, 98.16] |
| 4 | No ResNet | 98.77 [98.45, 99.05] | **99.94** [99.81, 100.00] | 98.02 [97.35, 98.55] |
| 5 | No SVM | 98.75 [98.30, 99.11] | 99.63 [99.31, 99.88] | 97.98 [97.36, 98.51] |
| 6 | Hudgins feature set | 98.83 [98.38, 99.21] | 99.56 [99.13, 99.94] | **98.19** [97.56, 98.70] |

### Window

| # | Ablation | Mean acc | Balanced acc | Macro-F1 | Pooled acc |
|---|----------|----------|--------------|----------|------------|
| 1 | No MLP | **98.89** | **98.84** | **98.80** | **98.88** |
| 2 | No ExtraTrees | 98.86 | 98.79 | 98.76 | 98.84 |
| 3 | No LDA | 98.55 | 98.48 | 98.45 | 98.49 |
| 4 | No ResNet | 98.77 | 98.73 | 98.70 | 98.74 |
| 5 | No SVM | 98.75 | 98.64 | 98.58 | 98.75 |
| 6 | Hudgins feature set | 98.83 | 98.75 | 98.73 | 98.81 |

### Whole repetition

| # | Ablation | Mean acc | Balanced acc | Macro-F1 | Pooled acc |
|---|----------|----------|--------------|----------|------------|
| 1 | No MLP | 99.75 | 99.75 | 99.74 | 99.75 |
| 2 | No ExtraTrees | 99.75 | 99.75 | 99.74 | 99.75 |
| 3 | No LDA | 99.56 | 99.56 | 99.55 | 99.56 |
| 4 | No ResNet | **99.94** | **99.94** | **99.93** | **99.94** |
| 5 | No SVM | 99.63 | 99.63 | 99.61 | 99.63 |
| 6 | Hudgins feature set | 99.56 | 99.56 | 99.55 | 99.56 |

### Raw window

| # | Ablation | Mean acc | Balanced acc | Macro-F1 | Pooled acc |
|---|----------|----------|--------------|----------|------------|
| 1 | No MLP | 98.08 | 98.12 | 98.07 | 98.02 |
| 2 | No ExtraTrees | 98.10 | 98.13 | 98.07 | 98.05 |
| 3 | No LDA | 97.62 | 97.66 | 97.61 | 97.53 |
| 4 | No ResNet | 98.02 | 98.05 | 98.00 | 97.94 |
| 5 | No SVM | 97.98 | 97.99 | 97.93 | 97.97 |
| 6 | Hudgins feature set | **98.19** | **98.16** | **98.12** | **98.15** |

