---
title: "Cortical eigenmode coordinates provide compact subject-level signatures across structural MRI, resting-state fMRI, and EEG"
title_zh: 皮层本征模坐标提供跨结构MRI、静息态fMRI和EEG的紧凑受试者级特征
authors: "Park, H. G., Tarpey, T."
date: 2026-05-28
pdf: "https://www.biorxiv.org/content/10.64898/2026.05.25.726064v1.full.pdf"
tags: ["query:eeg-priors"]
score: 8.0
evidence: 皮层本征模坐标作为EEG源分析的几何对齐先验
tldr: 多模态脑影像分析面临数据空间不统一的问题。本文提出皮层拉普拉斯-贝尔特拉米本征模坐标作为共享几何对齐语言，统一结构MRI、静息态fMRI和脑电图。在MPI-LEMON数据集上，本征模坐标表示相比传统方法在年龄预测任务中达到更高性能且维度更紧凑。GEMF模型进一步提取低维共享因子，提供了可解释的模态共享与特异性成分。该框架为构建跨模态的紧凑、可解释受试者级别脑特征奠定了实用基础。
source: biorxiv
selection_source: fresh_fetch
motivation: 多模态脑影像数据缺乏统一的几何对齐语言，导致难以构建跨模态的紧凑、可解释受试者级别特征。
method: 采用皮层拉普拉斯-贝尔特拉米本征模坐标表示sMRI、rs-fMRI和EEG，并使用PCA和几何本征模多视图分解（GEMF）提取共享与特异因子。
result: 本征模坐标表示在年龄预测中优于传统方法，多模态本征模坐标PCA性能领先，GEMF以更低维度保持竞争力并输出可解释因子。
conclusion: 皮层本征模坐标可作为多模态脑影像数据实现紧凑、可解释、对齐的受试者特征的有效基础框架。
---

## 摘要
多模态神经影像学的一个实际障碍是，结构MRI、fMRI和EEG往往在模态特定的空间中进行分析，或简化为基于图谱和传感器的摘要，限制了通用、可解释的受试者级脑特征的构建。我们评估了皮层拉普拉斯-贝尔特拉米本征模坐标作为结构MRI（sMRI）、静息态fMRI（rs-fMRI）和EEG的共享几何对齐语言。在此框架中，sMRI形态测量场由皮层本征模系数表示，rs-fMRI由本征模时间序列系数间的协方差表示，EEG由模态-频率-条件摘要表示。利用马克斯·普朗克研究所莱比锡心智-大脑-身体数据集（MPI-LEMON），我们比较了单模态本征模坐标摘要、多模态皮层本征模坐标PCA、传统的基于图谱/传感器的PCA和岭表示，以及几何本征模多视图分解（GEMF）。GEMF是一种结构化分解方法，在分离共享变异与模态特异性变异的同时，保留了数据对象的模态原生组织。本征模坐标表示产生了紧凑的受试者级特征，对实足年龄和次要认知结果具有强大的外部效度。多模态皮层本征模坐标PCA是表现最佳的方法之一，在中等维度下达到较高的年龄预测性能，并且始终优于传统的低维PCA。GEMF选择了更低的共享表示维度，并保持竞争力，同时提供了可解释的共享和模态特异性因素。这些发现支持皮层本征模坐标作为紧凑、可解释且多模态对齐的受试者级脑特征的实用基础。

## Abstract
A practical barrier in multimodal neuroimaging is that structural MRI, fMRI, and EEG are often analyzed in modality-specific spaces or reduced to atlas- and sensor-based summaries, limiting the construction of common, interpretable subject-level brain signatures. We evaluate cortical Laplace-Beltrami eigenmode coordinates as a shared geometry-aligned language for structural MRI (sMRI), resting-state fMRI (rs-fMRI), and EEG. In this framework, sMRI morphometric fields are represented by cortical eigenmode coefficients, rs-fMRI by covariance among eigenmode time-series coefficients, and EEG by mode-frequency-condition summaries.

Using the Max Planck Institute Leipzig Mind-Brain-Body dataset (MPI-LEMON), we compared unimodal eigenmode-coordinate summaries, multimodal cortical eigenmode-coordinate PCA, conventional atlas/sensor-based PCA and ridge representations, and geometric eigenmode multiview factorization (GEMF). GEMF is a structured decomposition that preserves the modality-native organization of the data objects while separating shared from modality-specific variation. Eigenmode-coordinate representations yielded compact subject-level signatures with strong external validity for chronological age and a secondary cognitive outcome. Multimodal eigenmode-coordinate PCA was among the strongest-performing approaches, reached high age-prediction performance at moderate dimension, and consistently outperformed conventional low-dimensional PCA. GEMF selected an even lower-dimensional shared representation and remained competitive with the benefit of providing interpretable shared and modality-specific factors.

These findings support cortical eigenmode coordinates as a practical foundation for compact, interpretable, and multimodally aligned subject-level brain signatures.