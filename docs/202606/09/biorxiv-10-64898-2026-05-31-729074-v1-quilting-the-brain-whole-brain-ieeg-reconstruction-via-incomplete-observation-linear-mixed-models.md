---
title: "Quilting the Brain: Whole-Brain iEEG Reconstruction via Incomplete Observation Linear Mixed Models"
title_zh: 拼接大脑：基于不完全观测线性混合模型的全脑iEEG重建
authors: "Wang, Y., Li, M., Bringas Vega, M. L., Valdes-Sosa, P. A."
date: 2026-06-03
pdf: "https://www.biorxiv.org/content/10.64898/2026.05.31.729074v1.full.pdf"
tags: ["query:eeg-priors"]
score: 6.0
evidence: 利用线性混合模型中的统计先验从稀疏iEEG重建全脑源活动
tldr: 颅内脑电图（iEEG）因临床植入策略导致观测碎片化，形成“覆盖悖论”，无法获得全脑映射。本研究提出不完全观测线性混合效应模型（IOLMM），利用超高维统计的Sure Independence Screening（SIS）区分真实信号与容积传导伪影，并通过层次模型分离群体固定效应与个体随机效应。基于MNI Open iEEG Atlas的106名患者数据，成功重建了睡眠阶段依赖的皮层源功率图，恢复了NREM慢波活动的额叶优势与电生理层级特征。该工作建立了首个基于iEEG的皮层表面规范化电生理图谱，弥合了微观电生理与宏观系统神经科学之间的鸿沟。
source: biorxiv
selection_source: fresh_fetch
motivation: 解决iEEG观测碎片化导致的全脑映射缺失问题，突破临床采样局限。
method: 提出IOLMM，结合SIS几何筛选与层次混合效应模型，实现碎片观测到全脑源活动的重建。
result: 在106名患者数据上成功重构Wake、N2、N3、REM状态的皮层源功率，复现NREM慢波额叶优势等已知特征。
conclusion: 建立了首个基于iEEG的皮层表面规范电生理图谱，为癫痫病灶检测提供定量参考。
---

## 摘要
高时空分辨率的人类脑功能成像受到非侵入式成像的物理限制以及侵入式电生理稀疏采样的约束。尽管颅内脑电图（iEEG）能够以毫米级精度捕捉局部场电位，但临床植入策略导致了一种“覆盖悖论”：观测局限于互不相连的患者特定区域，大部分皮层未被观测。本研究引入了不完全观测线性混合效应模型（IOLMM），这是一种统计框架，通过将碎片化的观测“拼接”为连续的全脑源活动图来解决这一悖论。我们的方法整合了两项创新：（1）从超高维统计中改进的确定独立筛选（SIS），用于区分真实生理信号与容积传导的“伪影源”；（2）分层IOLMM，将群体水平的生理固定效应与受试者特定的工具随机效应解耦，解决了困扰iEEG群体分析的尺度模糊问题。应用于MNI Open iEEG Atlas，该框架通过跨清醒、N2、N3和REM状态的睡眠阶段依赖性皮层源功率重建进行验证，从106名患者的碎片化记录中恢复了NREM慢波活动的前额优势以及分级电生理层级。这项工作建立了首个源自iEEG的皮层表面级规范电生理图谱，为检测和预测致痫灶提供了定量参考，并弥合了电生理微观精度与系统神经科学宏观范围之间的差距。

亮点
O_LI解决覆盖悖论：一种新颖的IOLMM统计框架将稀疏、非重叠的iEEG数据拼接为统一的全脑概率图。
C_LIO_LI几何筛选：利用皮层几何本征模改进高维确定独立筛选（SIS），有效过滤逆解中的虚假伪影源。
C_LIO_LI稳健协调：将群体水平生理固定效应与受试者特定随机效应解耦，解决了异质多中心记录中固有的尺度模糊。
C_LIO_LI生物学验证：通过重建睡眠阶段依赖性皮层源功率图，从碎片化记录中恢复NREM和REM睡眠的已知电生理特征，在实际多中心iEEG数据上验证了该框架。
C_LI

## Abstract
Mapping human brain function at high spatiotemporal resolution is constrained by the physical limitations of non-invasive imaging and the sparse sampling of invasive electrophysiology. While intracranial electroencephalography (iEEG) captures local eld potentials with millimeter precision, clinical implantation strategies result in a "coverage paradox" : observations are restricted to disjoint, patient-specific patches, leaving most of the cortex unobserved. This study introduces the Incomplete Observation Linear Mixed-Effect Model (IOLMM), a statistical framework that resolves this paradox by "quilting" fragmented observations into continuous, whole-brain source activity maps. Our approach integrates two innovations: (1) Sure Independence Screening (SIS) adapted from ultra-high-dimensional statistics to distinguish true physiological signals from volume-conducted "ghost sources"; (2) a hierarchical IOLMM that decouples group-level physiological fixed effects from subject-specific instrumental random effects, solving the scaling ambiguities that plague iEEG group analyses. Applied to the MNI Open iEEG Atlas, the framework is validated through sleep stage-dependent cortical source power reconstruction across Wake, N2, N3, and REM states, recovering the frontal predominance of NREM slow-wave activity and the graded electrophysiological hierarchy from fragmented recordings of 106 patients. This work establishes the first cortical surface-level normative electrophysiological atlas derived from iEEG, providing a quantitative reference for detecting and predicting epileptogenic lesions and bridging the gap between the microscopic precision of electrophysiology and the macroscopic scope of systems neuroscience.

HighlightsO_LISolving the Coverage Paradox: A novel IOLMM statistical framework quilts sparse, non-overlapping iEEG data into a unified whole-brain probabilistic map.
C_LIO_LIGeometric Screening: Adapts high-dimensional Sure Independence Screening (SIS) using cortical geometric eigenmodes to effectively filter out spurious ghost sources in inverse solutions.
C_LIO_LIRobust Harmonization: Decouples group-level physiological fixed effects from subject-specific random effects, resolving scaling ambiguities inherent in heterogeneous multi-center recordings.
C_LIO_LIBiological Validation: Validates the framework on real multi-center iEEG data by reconstructing sleep stage-dependent cortical source power maps, recovering known electrophysiological signatures of NREM and REM sleep from fragmented recordings.
C_LI