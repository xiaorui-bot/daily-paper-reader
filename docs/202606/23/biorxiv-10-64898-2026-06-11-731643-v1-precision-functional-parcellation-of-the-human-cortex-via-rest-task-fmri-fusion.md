---
title: Precision Functional Parcellation of the Human Cortex via Rest-Task fMRI Fusion
title_zh: 通过静息态与任务态fMRI融合实现人脑皮层精确功能划分
authors: "Zhi, D., Du, J., Whitfield-Gabrieli, S., Diedrichsen, J., Ge, T."
date: 2026-06-16
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.11.731643v1.full.pdf"
tags: ["query:eeg-priors"]
score: 6.0
evidence: 使用fMRI的皮层分区提供了可用于EEG源定位的解剖脑区先验
tldr: 个体化皮层分区多基于静息态fMRI，忽视了任务态数据的互补信息。本文提出mRBM-HBP分层贝叶斯框架，通过多项受限玻尔兹曼机高效融合多源静息态和任务态fMRI，推断群组与个体分区。该方法计算成本低，任务数据提供状态特异性边界细化；融合图谱在个体数据有限时显著提升准确性和可靠性。结果表明，整合两类fMRI可增强人脑功能组织的精确映射。
source: biorxiv
selection_source: fresh_fetch
motivation: 现有皮层分区方法依赖静息态fMRI，未充分利用任务态数据，难以整合异构数据集，限制了个体化功能映射精度。
method: 提出mRBM-HBP分层贝叶斯框架，基于多项受限玻尔兹曼机建模空间依赖，实现静息态与任务态fMRI的高效融合及群组/个体分区推断。
result: mRBM-HBP性能与现有方法相当但计算成本大幅降低；任务态数据细化功能边界；融合图谱在个体数据有限时提升准确性与个体特异性。
conclusion: 整合静息态与任务态fMRI可增强脑功能组织精确映射，尤其在个体数据受限时具有显著优势。
---

## 摘要
个体特异性皮层划分能够表征常被群体图谱掩盖的脑网络组织，对基础神经科学和转化应用具有广泛意义。然而，现有方法主要依赖静息态fMRI，未能充分利用任务诱发数据（后者提供功能特化的补充信息）。这一局限性部分反映了整合异质数据集（在任务设计、样本量和皮层覆盖范围上存在差异）的挑战。本文提出mRBM-HBP（可扩展分层贝叶斯框架），该框架结合多项受限玻尔兹曼机建模空间依赖性，能够高效灵活地整合跨数据集的静息态与任务态fMRI，并推断群体和个体层级的皮层划分。我们证明，mRBM-HBP在保持与最优静息态划分方法相当性能的同时，大幅降低了计算成本。通过整合大规模任务fMRI数据集，我们导出基于任务的皮层划分，并证明静息态与任务条件揭示了基本一致的宏观网络，而任务数据则提供了状态特异的功能边界修正。此外，融合静息-任务的群体图谱提高了推断划分的准确性、可靠性和个体特异性，尤其在个体数据有限时更为显著。这些结果表明，整合静息态与任务态fMRI可增强脑功能组织的精确映射。

## Abstract
Individual-specific cortical parcellations enable the characterization of brain network organization that is often obscured by population-level atlases, with broad implications for both basic neuroscience and translational applications. However, existing methods rely primarily on resting-state fMRI and underutilize task-evoked data, which provide complementary information about functional specialization. This limitation partly reflects the challenge of integrating heterogeneous datasets that differ in task design, sample size, and cortical coverage. Here, we present mRBM-HBP, a scalable hierarchical Bayesian framework that incorporates a multinomial restricted Boltzmann machine to model spatial dependencies, enabling efficient and flexible integration of resting-state and task fMRI across diverse datasets and inference of both group-level and individual-level cortical parcellations. We show that mRBM-HBP achieves performance comparable to state-of-the-art resting-state-based parcellation methods while substantially reducing computational cost. By integrating large-scale task-fMRI datasets, we derive a task-based parcellation and demonstrate that resting-state and task conditions reveal largely consistent macroscopic networks, while task data provide state-specific refinements of functional boundaries. Moreover, a fused rest-task group-level atlas improves the accuracy, reliability, and individual specificity of inferred parcellations, particularly when individual-level data are limited. These results indicate that integrating resting-state and task fMRI enhances precision mapping of functional brain organization.