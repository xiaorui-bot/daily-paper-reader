---
title: Bandwidth-aware fusion of resting-state EEG-fMRI connectivity in cortical eigenmode space
title_zh: 皮层本征模态空间中静息态 EEG-fMRI 连接性的带宽感知融合
authors: "Park, H. G."
date: 2026-05-19
pdf: "https://www.biorxiv.org/content/10.64898/2026.05.15.725408v1.full.pdf"
tags: ["query:eeg-priors"]
score: 9.0
evidence: 使用皮层拉普拉斯-贝尔特拉米本征模作为EEG-fMRI融合的解剖先验
tldr: 针对EEG和fMRI连接性融合中模态带宽不匹配问题，提出在皮层Laplace-Beltrami本征模空间进行带宽感知融合。通过低秩分解共享网络因子和频率特定强度，并利用谱平滑正则化推断未观测频带。在MPI-LEMON队列中，融合表示支持年龄预测并产出可解释的多模态网络生物标志物，为个体差异研究提供新途径。
source: biorxiv
selection_source: fresh_fetch
motivation: EEG-fMRI连接性融合面临时空分辨率与带宽差异挑战，现有方法未充分利用其互补性。
method: 在皮层LB本征模基下将EEG/fMRI建模为共享潜在连接的部分观测，用低秩分解加谱平滑融合。
result: 在MPI-LEMON队列中，融合特征支持年龄预测并生成多视图可解释的皮层系统组成与振荡谱。
conclusion: 显式建模带宽差距实现原则性融合，为个体差异研究提供可靠多模态网络生物标志物。
---

## 摘要
我们引入了一种几何引导的、带宽感知的模型，用于融合静息态 EEG 和 fMRI 连接性，将每种模态视为对共享潜在皮层连接性结构的掩蔽、物理受限观测。两种模态在共享的皮层 Laplace-Beltrami (LB) 本征模态基中表示，该基提供了空间尺度的解剖学排序。在该坐标系中，fMRI 在广泛空间尺度上约束连接性，但仅在慢时间尺度上；而 EEG 则主要为粗空间模态提供频率分辨信息。我们通过一个潜在的空间-频谱连接性对象形式化这种互补性，并使用共享本征模态-网络因子以及受试者与频率特异性非负强度的低秩分解来估计它。估计由每种模态支持的区域驱动（EEG：宽频率下的粗空间模态；fMRI：低频下的宽空间模态），而未观测频带通过共享低秩结构和频谱平滑正则化进行推断。在 MPI-LEMON 队列中，融合表示产生了紧凑、可解释的受试者特征（fMRI 网络强度和 EEG 振荡总结），这些特征支持嵌套交叉验证下的样本外年龄预测，并通过皮层图谱、频谱剖面和参考图谱的系统组成总结实现连贯的多视图解释。这些结果表明，显式建模模态特异性带宽缺口能够实现原则性的 EEG-fMRI 连接性融合，并为个体差异研究中的多模态网络生物标志物提供了实用途径。

## Abstract
We introduce a geometry-informed, bandwidth-aware model for fusing resting-state EEG and fMRI connectivity by treating each modality as a masked, physics-limited observation of a shared latent cortical connectivity structure. Both modalities are represented in a shared cortical Laplace-Beltrami (LB) eigenmode basis that provides an anatomically grounded ordering of spatial scales. In this coordinate system, fMRI constrains connectivity across a broad range of spatial scales but only at slow timescales, whereas EEG provides frequency-resolved information primarily for coarse spatial modes. We formalize this complementarity through a latent spatio-spectral connectivity object and estimate it using a low-rank factorization with shared eigenmode-network factors and subject- and frequency-specific nonnegative strengths. Estimation is driven by the regions supported by each modality (EEG: coarse spatial modes across broad frequencies; fMRI: broad spatial modes at low frequencies), while unobserved bands are inferred through shared low-rank structure and spectral smoothness regularization. In the MPI-LEMON cohort, the fused representation yields compact, interpretable subject features (fMRI network strengths and EEG oscillatory summaries) that support out-of-sample age prediction under nested cross-validation, and coherent multi-view interpretation through cortical maps, spectral profiles, and atlas-referenced system composition summaries. These results demonstrate that explicitly modeling modality-specific bandwidth gaps enables principled EEG-fMRI connectivity fusion and provides a practical route to multimodal network biomarkers for individual-differences research.