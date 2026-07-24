---
title: Measurement Equivalence of On-Scalp OPM-MEG and Cryogenic MEG for Auditory and Somatosensory Cortical Mapping Across Development
title_zh: 头皮上OPM-MEG与低温MEG在听觉和体感皮层发育图谱中的测量等效性
authors: "Gaetz, W., O'Neill, G. C., Birnbaum, C., Cheung, T., Robets, T. P. L., Hughes, K. J., Knappe, S., Alem, O."
date: 2026-07-20
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.01.728862v2.full.pdf"
tags: ["query:eeg-priors"]
score: 6.0
evidence: 比较了等效电流偶极子源模型在听觉和体感皮层定位中的应用
tldr: 可穿戴OPM-MEG较传统SQUID-MEG更贴近头皮，但两者测量等价性未知。本研究在18名参与者（10-45岁）中同时记录听觉和体感诱发场，采用相同建模流程对比。结果表明两种系统定位的皮层发生器潜伏期一致，空间存在可预测的系统偏移（SQUID偏内侧约4mm），偶极矩差异由偏移解释，年龄效应在两种系统一致。这证明了OPM-MEG与SQUID-MEG的测量等价性，支持OPM-MEG用于感觉功能映射。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-01-728862-v2/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1669, \"height\": 962, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-01-728862-v2/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1709, \"height\": 1307, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-01-728862-v2/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1576, \"height\": 1482, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-01-728862-v2/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1659, \"height\": 1287, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-01-728862-v2/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1504, \"height\": 1415, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-06-01-728862-v2/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1845, \"height\": 250, \"label\": \"Table\"}, {\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-06-01-728862-v2/table-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1758, \"height\": 295, \"label\": \"Table\"}]"
motivation: 验证可穿戴OPM-MEG与传统SQUID-MEG在人脑感觉皮层映射中的测量等价性。
method: 对18名参与者（10-45岁）分别使用128通道OPM-MEG和275通道SQUID-MEG记录听觉和体感诱发场，以等效电流偶极子源模型比较。
result: 两种系统定位的听觉和体感皮层发生器潜伏期匹配；SQUID定位偏内侧约4mm，导致偶极矩偏大，但年龄效应（听觉随增龄增强）在两种系统一致。
conclusion: OPM-MEG与SQUID-MEG在感觉皮层功能映射中测量等价，支持OPM-MEG作为有效替代方案。
---

## 摘要
可穿戴光泵磁力计脑磁图（OPM-MEG）与传统低温SQUID-MEG相比，减小了传感器到皮层的距离，但两种技术是否产生等效的神经生理学结论仍不清楚。我们在18名参与者（10-45岁）中，使用128传感器FieldLine HEDscan OPM-MEG系统和275通道CTF SQUID-MEG系统记录了听觉和体感诱发电位。通过相同的预处理和建模程序估计等效电流偶极子源模型，并使用配对置换检验进行比较。两个系统均定位了标准的听觉和体感皮层发生器，具有匹配的峰值潜伏期和适度的跨系统空间差异。听觉源在SQUID-MEG定位中呈现一致的内侧偏差，而体感源则表现出小的系统性偏移（约4毫米），表明是稳定的坐标差异而非定位误差。SQUID-MEG的偶极矩更大，OPM-MEG的拟合优度更高；然而，偶极矩的增加可由内侧定位偏差解释，表明是逆模型效应而非生理学不一致。听觉偶极矩在两个系统中均随年龄增长而增加，而体感反应则无年龄相关变化。总之，这些观察表明不同平台间保留了发育生理学。这些发现表明，OPM-MEG和SQUID-MEG能够恢复相同的皮层发生器，并支持等效的生物学解释，尽管存在可预测的几何相关坐标差异。因此，OPM-MEG是一种测量等效的MEG实现，适用于感觉功能图谱。

## Abstract
Wearable optically pumped magnetometer magnetoencephalography (OPM-MEG) reduces sensor-to-cortex distance compared with conventional cryogenic SQUID-MEG, but whether the two technologies yield equivalent neurophysiological conclusions remains unclear. We recorded auditory and somatosensory evoked fields in 18 participants (10-45 years) using a 128-sensor FieldLine HEDscan OPM-MEG system and a 275-channel CTF SQUID-MEG system within the same individuals. Equivalent current dipole source models were estimated using identical preprocessing and modeling procedures and compared using paired permutation testing.

Both systems localized canonical auditory and somatosensory cortical generators with matched peak latencies and modest cross-system spatial differences. Auditory sources showed a consistent medial bias in SQUID-MEG localization, whereas somatosensory sources exhibited a small systematic offset ([~]4 mm), indicating stable coordinate differences rather than localization error. Dipole moments were larger for SQUID-MEG and goodness-of-fit higher for OPM-MEG; however, the increased moment was explained by a medial localization bias, demonstrating inverse-model effects rather than physiological disagreement. Auditory dipole moment increased with age in both systems, whereas somatosensory responses showed no age-related change. Together, these observations indicate preserved developmental physiology across platforms.

These findings demonstrate that OPM-MEG and SQUID-MEG recover the same cortical generators and support equivalent biological interpretations despite predictable geometry-dependent coordinate differences. OPM-MEG therefore represents a measurement-equivalent implementation of MEG suitable for sensory functional mapping.