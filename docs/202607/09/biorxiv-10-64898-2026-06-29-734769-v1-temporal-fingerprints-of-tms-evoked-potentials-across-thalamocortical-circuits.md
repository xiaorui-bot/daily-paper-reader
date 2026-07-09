---
title: Temporal fingerprints of TMS-evoked potentials across thalamocortical circuits
title_zh: 跨丘脑-皮层环路的TMS诱发电位的时间指纹
authors: "Hassan, G., Gaglioti, G., Furregoni, G., Focacci, E., Porro, M., Bernardelli, L., Calcagno, A., Massimini, M., Sarasso, S., Rosanova, M., Casarotto, S."
date: 2026-07-02
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.29.734769v1.full.pdf"
tags: ["query:eeg-priors"]
score: 6.0
evidence: 研究了额叶、顶叶、枕叶皮层的区域特异性TMS诱发电位，提供了脑区先验
tldr: 经颅磁刺激诱发电位（TEP）是研究皮层动态的重要手段，但缺乏对不同脑区TEP形态的系统分析。本文对40名受试者分别刺激枕叶、顶叶和额叶皮层，自动计算TEP的峰峰值幅度、潜伏期和峰间间隔。结果发现枕叶TEP幅度最大、潜伏期最长；沿后-前轴潜伏期和峰间间隔递减，体现不同网络的重入动力学差异。该工作揭示了TEP形态特征反映刺激网络特性，并提供了Python工具用于表征皮层反应性。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-29-734769-v1/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1609, \"height\": 1843, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-29-734769-v1/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1489, \"height\": 1318, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-29-734769-v1/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1549, \"height\": 1597, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-29-734769-v1/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1697, \"height\": 1561, \"label\": \"Figure\"}]"
motivation: 系统探索不同脑区TMS诱发脑电形态特征，建立类似感觉诱发电位的区域特异性指标。
method: 对40名受试者枕、顶、额叶TMS，自动计算TEP的峰值幅度、潜伏期和峰间间隔。
result: 枕叶TEP幅度最大、潜伏期最长；后-前轴潜伏期和峰间间隔递减，反映不同网络动态。
conclusion: TEP形态由刺激网络特性决定，早期幅度反映局部募集，后期时间特征跟踪节律活动。
---

## 摘要
背景经颅磁刺激（TMS）诱发的脑电图（EEG）电位为皮层动力学提供了直接窗口。然而，对其形态特征的系统探索（类似于感觉诱发电位）仍缺乏，尤其是对于运动皮层以外的刺激。

目的从TMS诱发电位（TEP）的时间过程中获取额叶、顶叶和枕叶网络的区域特异性特性。

材料与方法我们实施并应用了一种自动程序，计算了40名神经典型受试者在左侧枕叶（n=25）、顶叶（n=25）和额叶（n=25）皮层刺激下记录的TEP的峰-峰振幅、峰潜伏期和峰间间隔。

结果枕叶TEP表现出最大的峰-峰振幅和第一个波形成分的最长潜伏期，这独立于刺激强度，并与招募一大片密集互连的神经元相一致。对于较晚的成分，潜伏期和峰间间隔沿后-前轴系统性减小，反映了从α波主导的枕叶回路到额叶皮层与皮层下结构之间紧密耦合环路的逐渐加快的递归动力学。顶叶TEP显示出中等振幅和潜伏期测量值，与上顶叶皮层异质的细胞构筑和连接组织一致。

结论我们的发现表明，TEP形态由受刺激网络的不同特性塑造，早期振幅反映了局部招募的程度，而较晚的时间特征追踪了递归活动的节律。这项工作提供了一种基于机制且易于实践的方法，也以基于Python的工具形式发布，允许表征不同脑状态和人群的皮层反应性。

## Abstract
BackgroundElectroencephalographic (EEG) potentials evoked by transcranial magnetic stimulation (TMS) offer a direct window into cortical dynamics. Yet, a systematic exploration of their morphological features, analogous to sensory-evoked potentials, is lacking, especially for stimulation outside the motor cortex.

AimTo obtain region-specific properties of frontal, parietal and occipital networks from the time course of TMS-evoked potentials (TEPs).

Materials and MethodsWe implemented and applied an automatic procedure to compute peak-to-peak amplitude, peak latency, and inter-peak interval of TEPs recorded from 40 neurotypical subjects stimulated over left occipital (n=25), parietal (n=25), and frontal (n=25) cortices.

ResultsOccipital TEPs showed the largest peak-to-peak amplitude and longest latency of the first waveform component, independently of stimulation intensity and consistent with the recruitment of a large patch of densely interconnected neurons. Concerning later components, both latency and inter-peak interval systematically decreased along the posterior-to-anterior axis, reflecting progressively faster recurrent dynamics from the alpha-dominated occipital circuitry to the tightly coupled loops between frontal cortex and subcortical structures. Parietal TEPs showed intermediate amplitude and latency measures, consistent with the heterogeneous cytoarchitectonic and connectional organization of the superior parietal cortex.

ConclusionsOur findings suggest that TEP morphology is shaped by the distinct properties of the stimulated networks, with early amplitude reflecting the extent of local recruitment and later temporal features tracking the rhythm of recurrent activity. This work offers a mechanistically grounded and practically accessible approach, also released as a Python-based tool, that allows to characterize cortical reactivity across different brain-states and populations.