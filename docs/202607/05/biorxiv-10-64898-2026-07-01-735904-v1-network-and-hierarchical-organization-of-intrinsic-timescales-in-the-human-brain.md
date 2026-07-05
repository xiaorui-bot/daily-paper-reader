---
title: Network and hierarchical organization of intrinsic timescales in the human brain
title_zh: 人脑内在时间尺度的网络与层级组织
authors: "Krause, B. M., Bublitz, E. F., Dappen, E. R., Kawasaki, H., Nourski, K. V., Banks, M. I."
date: 2026-07-02
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.01.735904v1.full.pdf"
tags: ["query:eeg-priors"]
score: 7.0
evidence: 利用MNI坐标投影分配层级位置，为iEEG分析提供解剖先验
tldr: 人脑内在神经时间尺度反映信息维持时长，初级感觉区短而高级联合区长。本研究利用颅内脑电图，通过频谱参数化提取非周期成分估计时间尺度，并基于功能连接扩散图嵌入定义皮层层级位置。结果发现时间尺度随层级单调递增，并在网络枢纽中最大；睡眠状态动态调节层级组织，非快速眼动期时间尺度增大且层级梯度消失。
source: biorxiv
selection_source: fresh_fetch
motivation: 揭示皮层层级与内在时间尺度的关系，并探究睡眠等脑状态如何动态调节这一层级组织。
method: 从46名患者的颅内脑电图记录中提取非周期功率谱，通过扩散图嵌入将电极位点映射到层级位置，并计算功能连接拓扑指标。
result: 时间尺度随层级升高而增加；网络枢纽（强且均匀的连接）表现出最长的时间尺度；睡眠中层级梯度在REM和N2/N3期消失，因低级区时间尺度增大。
conclusion: 时间尺度层级组织由网络拓扑结构塑造，并受脑状态动态调节，为理解大脑信息处理的时空整合提供新视角。
---

## 摘要
内在神经时间尺度表征信息在神经回路中维持的特征持续时间。证据表明，神经时间尺度在皮层层级中系统性地变化，初级感觉区域的时间尺度较短，而高级联合区域的时间尺度较长。在以往研究中，层级结构被分类定义、解剖定义，或基于扩散映射嵌入（DME）从静息态功能磁共振成像（fMRI）功能连接的主梯度推导得出。本文通过将MNI坐标投影到由人类连接组计划静息态fMRI数据导出的该嵌入空间，为个体人类颅内脑电图（iEEG）记录位点分配层级位置。我们通过光谱参数化提取局部场电位功率谱的非周期性成分，从而从成年神经外科患者（n=46，25名女性）的静息态iEEG记录中估计神经时间尺度。时间尺度随层级位置单调增加，并与从参与者iEEG功能连接的DME导出的两个感兴趣区域（ROI）层面网络拓扑测量相关：平均功能连接更强的ROI表现出更长的时间尺度，作为枢纽（由接近嵌入空间中心定义）的ROI也是如此。最后，时间尺度随睡眠阶段变化，在非快速眼动（NREM）期间最慢，在清醒和快速眼动（REM）期间最快。清醒和N1期存在的层级梯度在REM、N2和N3睡眠期间不再被检测到，这是由于层级较低水平的时间尺度选择性增加所致。本研究提出了一种可应用于iEEG数据的层级新度量，建立了人脑iEEG中神经时间尺度、皮层层级与网络拓扑之间的直接联系，并证明这种层级组织受大脑状态动态调节。

意义声明大脑同时在多个时间尺度上处理信息，不同皮层区域特化于快速感觉处理或缓慢的语境整合。我们通过人类颅内电生理记录测量内在神经时间尺度，并应用一种新方法将每个记录位点定位在皮层层级上。时间尺度从感觉区域到联合区域系统性增加，并在网络枢纽（即与大脑其他部分均匀广泛连接的区域）中最长。在睡眠期间，这种层级组织未被检测到，感觉区域时间尺度增加最大。这些发现推进了我们关于大脑时间组织如何由网络架构塑造并受大脑状态调节的理解。

## Abstract
Intrinsic neural timescales represent the characteristic duration over which information is maintained in neuronal circuits. Evidence suggests that neural timescales vary systematically across the cortical hierarchy, with shorter timescales in primary sensory areas and longer timescales in higher-order association regions. In previous studies, hierarchy has been defined categorically, anatomically, or from the principal gradient of resting-state fMRI functional connectivity derived using diffusion map embedding (DME). Here, we assign hierarchical position to individual human intracranial electroencephalography (iEEG) recording sites by projecting their MNI coordinates onto this embedding space, derived from Human Connectome Project resting-state fMRI data. We estimated neural timescales from resting-state iEEG recordings in adult neurosurgical patients (n=46, 25 female) by extracting the aperiodic component of the local field potential power spectrum using spectral parameterization. Timescales increased monotonically with hierarchical position and associated with two region of interest (ROI)-level measures of network topology derived from DME of participants iEEG functional connectivity: ROIs with stronger mean functional connectivity exhibited longer timescales, as did ROIs functioning as hubs, defined by proximity to the center of embedding space. Finally, timescales varied with sleep stage, with slowest values during NREM and fastest during wake and REM. The hierarchical gradient present during wake and N1 was no longer detected during REM, N2, and N3 sleep, driven by a selective increase in timescales at lower levels of the hierarchy. This work presents a novel metric of hierarchy that can be applied to iEEG data, establishes a direct link between neural timescales, cortical hierarchy, and network topology in human iEEG, and demonstrates that this hierarchical organization is dynamically modulated by brain state.

Significance StatementThe brain processes information across multiple timescales simultaneously, with different cortical regions specialized for fast sensory processing or slow integration of context. We measured intrinsic neural timescales from human intracranial electrophysiological recordings and applied a novel method to locate each recording site along the cortical hierarchy. Timescales increased systematically from sensory to association areas, and were longest in network hubs, i.e., regions that are uniformly and widely connected to the rest of the brain. During sleep, this hierarchical organization was not detected, with sensory areas showing the largest increases in timescale. These findings advance our understanding of how the brains temporal organization is shaped by network architecture and modulated by brain state.