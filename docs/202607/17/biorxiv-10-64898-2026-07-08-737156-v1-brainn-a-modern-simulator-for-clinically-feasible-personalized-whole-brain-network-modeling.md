---
title: "BraiNN: A Modern Simulator for Clinically Feasible Personalized Whole-Brain Network Modeling"
title_zh: BraiNN：一种用于临床可行性个性化全脑网络建模的现代模拟器
authors: "Fasse, A., Billi, C., Garvalov, V., Morvan, M., Newton, T., Kuster, N., Neufeld, E."
date: 2026-07-13
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.08.737156v1.full.pdf"
tags: ["query:eeg-priors"]
score: 7.0
evidence: 全脑网络建模与EEG关联，可整合解剖先验
tldr: 个性化全脑网络建模需实现患者仿真的脑动力学模拟，但现有工具计算成本过高。本文提出BraiNN，基于JAX框架，利用GPU/TPU加速和XLA编译，集成Jansen-Rit模型和皮层表面网格，通过贝叶斯优化与梯度精化混合方法进行个性化参数拟合。在单个消费级GPU上，仅需2-3小时即可完成EEG驱动的谱拟合，相比传统方法提速2-3个数量级。该工作使临床可行的个性化数字脑建模成为可能。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-08-737156-v1/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 891, \"height\": 571, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-08-737156-v1/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1664, \"height\": 907, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-08-737156-v1/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 894, \"height\": 534, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-08-737156-v1/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 904, \"height\": 517, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-08-737156-v1/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 901, \"height\": 518, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-08-737156-v1/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 901, \"height\": 518, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-08-737156-v1/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 896, \"height\": 518, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-08-737156-v1/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1842, \"height\": 915, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-08-737156-v1/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 867, \"height\": 556, \"label\": \"Table\"}, {\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-08-737156-v1/table-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 898, \"height\": 297, \"label\": \"Table\"}]"
motivation: 解决现有全脑神经质量模型框架在临床时间尺度上计算效率过低的问题。
method: 提出JAX加速的BraiNN框架，结合区域Jansen-Rit网络、皮层网格模型及互易性EEG正向建模，采用贝叶斯优化与梯度精化混合策略进行个性化拟合。
result: 在单GPU上2-3小时完成8维参数空间EEG谱拟合，速度提升2-3个数量级，并精确再现Jansen-Rit网络动力学。
conclusion: BraiNN将个性化高细节全脑模型拟合时间从数天降至数小时，推进了临床个性化脑网络建模与数字孪生应用。
---

## 摘要
个性化全脑建模旨在通过实现患者特异性的大脑网络动力学模拟，来改变神经疾病的治疗规划。神经质量模型（NMM）在生物物理细节与计算成本之间提供了可处理的折衷，并可直接与EEG等宏观观测指标相关联。然而，将NMM扩展到具有真实连接性、传导延迟和皮层表面分辨率的全脑网络——并将其拟合到个体患者数据——所产生的计算需求，现有的框架无法在临床相关的时间尺度上满足。本文介绍了BraiNN，一个基于JAX的Python框架，用于大规模神经质量建模，通过利用GPU/TPU加速和XLA编译的数组计算，相比现有工具实现了高达两到三个数量级的加速。BraiNN将区域级Jansen-Rit网络与受试者特异性皮层表面网格（耦合神经质量模型）以及基于互易性的导联场（用于生物物理合理的EEG正向建模）相结合。其完全可微的计算图支持混合个性化流程，将用于全局参数探索的贝叶斯优化与基于梯度的细化相结合，在单个消费级GPU上约2-3小时内完成八维参数空间的EEG驱动谱拟合——而传统神经质量建模软件则需要数天。与已建立基准的数值验证确认，BraiNN忠实再现了Jansen-Rit网络的典型同步和分岔动力学。

通过将在消费级硬件上个性化高细节全脑表面模型的时间需求从数天减少到几小时，BraiNN使个性化大脑网络建模更接近临床实际应用。我们预计BraiNN将作为患者特异性数字孪生和EEG引导的神经调节规划的基础。

## Abstract
Personalized whole-brain modeling aims to transform treatment planning for neurological disorders by enabling patient-specific simulations of brain network dynamics. Neural mass models (NMMs) offer a tractable compromise between biophysical detail and computational cost and can be directly linked to macroscopic observables such as EEG. However, scaling NMMs to whole-brain networks with realistic connectivity, conduction delays, and cortical surface resolution--and fitting them to individual patient data--imposes computational demands that existing frameworks cannot meet at clinically relevant timescales. Here we introduce BraiNN, a JAX-based Python framework for large-scale neural mass modeling that achieves speedups of up to two to three orders of magnitude over existing tools by leveraging GPU/TPU-accelerated, XLA-compiled array computation. BraiNN combines a region-level Jansen-Rit network with a subject-specific cortical surface mesh of coupled neural mass models and biophysically grounded EEG forward modeling via reciprocity-based lead fields. Its fully differentiable computational graph enables a hybrid personalization pipeline that pairs Bayesian optimization for global parameter exploration with gradient-based refinement, completing EEG-driven spectral fitting of an eight-dimensional parameter space in approximately 2-3 hours on a single consumer GPU--compared to multiple days with conventional neural mass modeling software. Numerical verification against established benchmarks confirms that BraiNN faithfully reproduces canonical synchronization and bifurcation dynamics of Jansen-Rit networks.

By reducing the time requirements for personalizing a high-detail whole-brain surface model from days to a few hours on consumer-grade hardware, BraiNN brings personalized brain network modeling closer to practical use in clinical contexts. We anticipate that BraiNN will serve as a foundation for patient-specific digital twins and EEG-guided neuromodulation planning.