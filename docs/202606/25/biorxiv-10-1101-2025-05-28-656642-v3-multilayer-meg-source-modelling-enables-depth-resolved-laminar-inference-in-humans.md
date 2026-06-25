---
title: Multilayer MEG source modelling enables depth-resolved laminar inference in humans
title_zh: 多层脑磁图源建模实现人类深度分辨层状推断
authors: "Szul, M. J., Maspoli, M., Shelepenkov, D., Agarwal, I., Moreau, Q., Gailhard, S., Ferez, M., Fernandez Pujol, C., Zhu, Y., Hiba, B., Daligault, S., Lamberton, F., Schwartz, D., Mattout, J., Bonnefond, M., Dykstra, A. R., Bestmann, S., Barnes, G. R., Bonaiuto, J. J."
date: 2026-06-24
pdf: "https://www.biorxiv.org/content/10.1101/2025.05.28.656642v3.full.pdf"
tags: ["query:eeg-priors"]
score: 7.0
evidence: 多层MEG源重建利用皮层解剖先验实现层状分辨
tldr: 神经活动层流级解析对理解皮层计算至关重要，但现有无创方法仅能粗略区分深浅层。本文提出多层MEG源重建框架，通过系统模拟评估深度分辨的可行性，发现信噪比、配准精度和柱取向是关键因素，且导引场可分性决定重建保真度。在三个独立数据集中，该框架成功识别出与视觉和感觉运动环路中典型前馈、反馈模式一致的层流激活模式。该工作为连接侵入性电生理与人类神经影像提供了新途径。
source: biorxiv
selection_source: fresh_fetch
motivation: 现有无创神经成像方法缺乏对皮层层流活动进行深度分辨的能力，限制了人类皮层计算的研究。
method: 开发多层MEG源重建框架，通过模拟和实证评估信噪比、配准精度及柱取向等条件对层流推断的影响。
result: 在三个独立数据集上，框架成功检测到与视觉及感觉运动回路中前馈/反馈典型模式一致的层流激活。
conclusion: 在有利条件下，MEG可支持深度分辨的层流推断，架起侵入性电生理与人类神经影像的桥梁。
---

## 摘要
层状水平的神经动力学对皮层计算至关重要。然而，在人类中，探测这种动力学的非侵入性方法仅限于深层和表层之间的粗略区分。在这里，我们提出了一个多层脑磁图源重建框架，并评估了实现深度分辨层状推断可能性的条件。通过模拟，我们系统地评估了脑磁图深度分辨率的极限，表明层状区分依赖于足够高的信噪比、精确的共配准以及准确的皮层柱方向估计。我们证明了皮层解剖的区域变异会影响重建保真度，其中导联场可分离性成为关键决定因素。然后，我们将这一框架应用于三个独立数据集的经验数据，并发现了与视觉和感觉运动回路中经典的前馈和反馈模式一致的层状激活模式，这支持了在有利条件下进行层状推断的合理性，并为桥接侵入性电生理学与人类神经影像学提供了机会。

## Abstract
Neural dynamics at the laminar level are critical for cortical computation. However, in humans, non-invasive methods to probe such dynamics have been limited to coarse distinctions between deep and superficial layers. Here, we present a multilayer magnetoencephalography source reconstruction framework and evaluate the conditions under which depth-resolved laminar inference may be feasible. Using simulations, we systematically assess the limits of magnetoencephalography depth resolution, showing that laminar discrimination depends on sufficiently high signal-to-noise ratio, precise co-registration, and accurate specification of cortical column orientation. We demonstrate that regional variations in cortical anatomy influence reconstruction fidelity, with lead-field separability emerging as a key determinant. We then apply this framework to empirical data from three independent datasets and find laminar activation patterns that align with canonical feedforward and feedback motifs in visual and sensorimotor circuits, supporting the plausibility of laminar inference under favorable conditions and offering opportunities to bridge invasive electrophysiology and human neuroimaging.