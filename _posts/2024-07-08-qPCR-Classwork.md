---
layout: post
title: qPCR Classwork
date: '2024-07-08'
categories: Protocols
tags: qPCR
---

# qPCR Data Analysis

Today, we calculated various values obtained from the qPCR data.

## Ct (Cycle Threshold) Values
Ct values indicate the number of cycles required for the fluorescent signal to exceed the background level. They are inversely proportional to the amount of target nucleic acid in the sample; lower Ct values indicate higher amounts of target nucleic acid.

|                      | ubi   | Rac1  | RhoA  | CDC42 | Rock1 | Vegf  | VegfR | RhoGap24l/2 |
| -------------------- | ----- | ----- | ----- | ----- | ----- | ----- | ----- | ----------- |
| DMSO Control         | 20.72 | 25.65 | 29.13 | 28.45 | 28.28 | 29.71 | 28.61 | 29.48       |
| Inhibitor Treatment  | 19.89 | 25.34 | 28.41 | 27.38 | 28.01 | 28.85 | 28.36 | 30.45       |

**Fig. 1** - Cycle Threshold values (Ct)

## ΔCt (Delta Ct) Values
ΔCt is the difference between the Ct value of the target gene and the Ct value of a reference gene (housekeeping gene). This normalization accounts for variations in the amount of starting material and the efficiency of the PCR reaction.

|                      | Rac1 | RhoA | CDC42 | Rock1 | Vegf | VegfR | RhoGap24l/2 |
| -------------------- | ---- | ---- | ----- | ----- | ---- | ----- | ----------- |
| DMSO Control         | 4.94 | 8.41 | 7.73  | 7.56  | 8.99 | 7.90  | 8.76        |
| Inhibitor Treatment  | 5.44 | 8.51 | 7.48  | 8.11  | 8.95 | 8.47  | 10.56       |

**Fig. 2** - Delta Cycle Threshold (Ct)

## ΔΔCt (Delta Delta Ct) Values
ΔΔCt is the difference between the ΔCt of the experimental sample and the ΔCt of the control sample. This comparative method allows for the calculation of relative gene expression levels.

| Genes | Rac1 | RhoA | CDC42  | Rock1 | Vegf   | VegfR | RhoGap24l/2 |
| ----- | ---- | ---- | ------ | ----- | ------ | ----- | ----------- |
| Ct    | 0.51 | 0.10 | -0.25  | 0.55  | -0.04  | 0.57  | 1.79        |

**Fig. 3** - Delta Delta Cycle Threshold (Ct)

## Quantification (Absolute or Relative)
Absolute Quantification: Provides the exact number of copies of the target nucleic acid in the sample by comparing Ct values to a standard curve generated from known concentrations of the target.

Relative Quantification: Measures changes in gene expression levels relative to a control sample, usually using the ΔΔCt method.

The fold change in gene expression is calculated using the 2^(-ΔΔCt) method.

| Genes | Rac1 | RhoA | CDC42 | Rock1 | Vegf | VegfR | RhoGap24l/2 |
| ----- | ---- | ---- | ----- | ----- | ---- | ----- | ----------- |
| RQ    | 0.72 | 0.94 | 1.17  | 0.70  | 1.03 | 0.69  | 0.32        |

**Fig. 4** - Fold Change
