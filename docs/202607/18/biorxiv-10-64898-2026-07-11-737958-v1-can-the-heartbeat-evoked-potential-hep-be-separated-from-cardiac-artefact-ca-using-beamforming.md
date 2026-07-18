---
title: Can the heartbeat-evoked potential (HEP) be separated from Cardiac Artefact (CA) using beamforming?
title_zh: 心跳诱发电位（HEP）能否通过波束成形与心电伪迹（CA）分离？
authors: "Virjee, R.-I., Kandasamy, R., Garfinkel, S. N., Yogarajah, M., Litvak, V., Carmichael, D."
date: 2026-07-17
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.11.737958v1.full.pdf"
tags: ["query:eeg-priors"]
score: 8.0
evidence: 波束成形利用解剖先验分离心跳诱发电位源
tldr: "心跳诱发电位(HEP)作为内感受神经标记，常被心电伪迹(CA)污染，头皮分析难以区分。本文首次验证LCMV波束成形可在源空间分离HEP与CA，通过模拟和实证EEG数据表明，在足够高信噪比下能高精度恢复HEP（相关系数>0.99，误差<6mm），并有效抑制CA。实证分析在右脑岛和前扣带回检测到显著HEP活动，并发现高血压患者与对照组在晚期窗的显著差异（p<0.05）。该方法为区分真实HEP与伪迹提供了可靠的源级途径。"
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-11-737958-v1/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1080, \"height\": 2441, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-11-737958-v1/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 943, \"height\": 1205, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-11-737958-v1/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1412, \"height\": 701, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-11-737958-v1/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 983, \"height\": 619, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-11-737958-v1/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1684, \"height\": 1739, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-11-737958-v1/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1671, \"height\": 1730, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-11-737958-v1/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1656, \"height\": 1689, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-11-737958-v1/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1323, \"height\": 537, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-11-737958-v1/fig-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 1284, \"height\": 613, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-11-737958-v1/fig-010.webp\", \"caption\": \"\", \"page\": 0, \"index\": 10, \"width\": 1280, \"height\": 600, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-11-737958-v1/fig-011.webp\", \"caption\": \"\", \"page\": 0, \"index\": 11, \"width\": 1640, \"height\": 1036, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-11-737958-v1/fig-012.webp\", \"caption\": \"\", \"page\": 0, \"index\": 12, \"width\": 1662, \"height\": 1348, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-11-737958-v1/fig-013.webp\", \"caption\": \"\", \"page\": 0, \"index\": 13, \"width\": 1639, \"height\": 1014, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-11-737958-v1/fig-014.webp\", \"caption\": \"\", \"page\": 0, \"index\": 14, \"width\": 1654, \"height\": 2061, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-11-737958-v1/fig-015.webp\", \"caption\": \"\", \"page\": 0, \"index\": 15, \"width\": 1657, \"height\": 655, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-11-737958-v1/fig-016.webp\", \"caption\": \"\", \"page\": 0, \"index\": 16, \"width\": 772, \"height\": 951, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-11-737958-v1/fig-017.webp\", \"caption\": \"\", \"page\": 0, \"index\": 17, \"width\": 767, \"height\": 968, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-11-737958-v1/fig-018.webp\", \"caption\": \"\", \"page\": 0, \"index\": 18, \"width\": 780, \"height\": 979, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-11-737958-v1/fig-019.webp\", \"caption\": \"\", \"page\": 0, \"index\": 19, \"width\": 774, \"height\": 987, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-11-737958-v1/fig-020.webp\", \"caption\": \"\", \"page\": 0, \"index\": 20, \"width\": 1654, \"height\": 2042, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-11-737958-v1/fig-021.webp\", \"caption\": \"\", \"page\": 0, \"index\": 21, \"width\": 774, \"height\": 807, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-11-737958-v1/fig-022.webp\", \"caption\": \"\", \"page\": 0, \"index\": 22, \"width\": 1654, \"height\": 685, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-11-737958-v1/fig-023.webp\", \"caption\": \"\", \"page\": 0, \"index\": 23, \"width\": 775, \"height\": 958, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-11-737958-v1/fig-024.webp\", \"caption\": \"\", \"page\": 0, \"index\": 24, \"width\": 772, \"height\": 962, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-11-737958-v1/fig-025.webp\", \"caption\": \"\", \"page\": 0, \"index\": 25, \"width\": 771, \"height\": 978, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-11-737958-v1/fig-026.webp\", \"caption\": \"\", \"page\": 0, \"index\": 26, \"width\": 770, \"height\": 982, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-11-737958-v1/fig-027.webp\", \"caption\": \"\", \"page\": 0, \"index\": 27, \"width\": 1412, \"height\": 842, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-11-737958-v1/fig-028.webp\", \"caption\": \"\", \"page\": 0, \"index\": 28, \"width\": 1623, \"height\": 1254, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-11-737958-v1/fig-029.webp\", \"caption\": \"\", \"page\": 0, \"index\": 29, \"width\": 1617, \"height\": 804, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-11-737958-v1/fig-030.webp\", \"caption\": \"\", \"page\": 0, \"index\": 30, \"width\": 1629, \"height\": 695, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-11-737958-v1/fig-031.webp\", \"caption\": \"\", \"page\": 0, \"index\": 31, \"width\": 1618, \"height\": 1832, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-11-737958-v1/fig-032.webp\", \"caption\": \"\", \"page\": 0, \"index\": 32, \"width\": 1625, \"height\": 1868, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-11-737958-v1/fig-033.webp\", \"caption\": \"\", \"page\": 0, \"index\": 33, \"width\": 1624, \"height\": 1836, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-11-737958-v1/fig-034.webp\", \"caption\": \"\", \"page\": 0, \"index\": 34, \"width\": 1626, \"height\": 1837, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-11-737958-v1/fig-035.webp\", \"caption\": \"\", \"page\": 0, \"index\": 35, \"width\": 1288, \"height\": 758, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-11-737958-v1/fig-036.webp\", \"caption\": \"\", \"page\": 0, \"index\": 36, \"width\": 1595, \"height\": 1838, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-11-737958-v1/fig-037.webp\", \"caption\": \"\", \"page\": 0, \"index\": 37, \"width\": 1617, \"height\": 1884, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-11-737958-v1/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1567, \"height\": 460, \"label\": \"Table\"}, {\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-11-737958-v1/table-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1362, \"height\": 934, \"label\": \"Table\"}, {\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-11-737958-v1/table-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1368, \"height\": 1226, \"label\": \"Table\"}, {\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-11-737958-v1/table-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1370, \"height\": 844, \"label\": \"Table\"}, {\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-11-737958-v1/table-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1368, \"height\": 1275, \"label\": \"Table\"}, {\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-11-737958-v1/table-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1371, \"height\": 855, \"label\": \"Table\"}, {\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-11-737958-v1/table-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1373, \"height\": 1278, \"label\": \"Table\"}]"
motivation: 可靠分离HEP与CA是内感受神经机制研究的关键，但头皮水平难以区分，需从源空间解决。
method: 使用LCMV波束成形对128通道EEG进行源重建，结合空域投影去除残余CA，通过模拟和实证数据验证。
result: "模拟中高SNR下恢复近乎完美（r>0.99，0mm误差）；实证中检测到右脑岛和前扣带回显著HEP，并发现高血压组与对照组在250-500ms窗的显著差异（p=0.040）。"
conclusion: LCMV波束成形能可靠分离HEP与CA，为内感受研究提供有效源级工具，优于传统头皮分析。
---

## 摘要
心跳诱发电位（HEP）是一种对心跳的皮层反应，也是内感受的神经标志物，越来越多地被认为具有临床相关性，但它在头皮上严重受到心电伪迹（CA）的污染，使得HEP与CA的可靠区分变得具有挑战性。由于HEP和心脏电位在解剖结构上不同，它们可能可以通过波束成形（一种源定位方法，能在抑制外部噪声和干扰的同时隔离特定位置的脑活动）分离。这里，首次尝试对EEG波束成形用于HEP源重建进行地面真实验证，旨在使用模拟EEG数据量化源波形恢复和空间定位精度。使用线性约束最小方差（LCMV）波束成形，研究了以下内容。(A) 为了测试波束成形是否能恢复已知信号，针对3个具有已知HEP波形的模型模拟了128通道EEG数据集：单个右侧脑岛（R-Ins）HEP（1），R-Ins和右侧前扣带皮层（R-ACC）中两个时间上不同的HEP（2），以及相同区域中两个时间上重叠的HEP（3）。通过将真实位置处的虚拟电极波形与已知真实输入波形进行相关分析来研究恢复情况。(B) 为了测试CA抑制，将从脑死亡个体等电位EEG中提取的CA（该CA具有有限的皮层活动）集成到模拟EEG数据中。对于每个模型，在有和没有CA的情况下，系统地改变源（-10至-50dB）和传感器（0至-30dB）信噪比（SNR）。(C) 然后将LCMV波束成形应用于来自高血压和焦虑个体的回顾性经验EEG数据（n=106）。在模拟和经验数据中，T检验比较了HEP主导窗口与早期CA主导窗口的功率。使用受试者特异性QRS波形及其时间导数进行零空间投影，以去除重建源波形中的残余CA。在模型1中，波束成形在无CA时实现了近乎完美的恢复（r>0.99，0mm误差），源SNR为-30dB，在有CA时仍然稳健（r=0.72-0.94，0-5.7mm误差）。在低SNR（<-20 dB；r<0.3，误差高达27mm）时恢复质量下降。模型2和3显示出类似的模式，但引入了从R-ACC到R-Ins的漏电。应用于经验数据时，波束成形在源空间的所有汇集数据中揭示了R-Ins和R-ACC中的显著HEP活动（p < 0.001）。当排除低SNR受试者时，LCMV波束成形还揭示了高血压组与对照组在晚期R-ACC窗口（R峰后250-500 ms）中的显著HEP差异（p = 0.040，d = 0.92）。QRS清理后，这种效应增强（p = 0.035，d = 0.96）。LCMV波束成形可以在源SNR足够高的情况下可靠地恢复模拟HEP，同时抑制CA。应用于经验数据时，LCMV波束成形从内感受区域（R-Ins和R-ACC）恢复了HEP活动，并且足够灵敏以检测有临床意义的组间差异。本研究提供了一种源级方法，用于将HEP活动与CA分离，而传感器级分析难以做到这一点。总之，LCMV波束成形和基于头皮的方法可以为真实的HEP活动提供汇聚证据。

## Abstract
The heartbeat-evoked potential (HEP), a cortical response to heartbeats and a neural marker of interoception, is increasingly considered clinically relevant, but is heavily contaminated by cardiac artefact (CA) on the scalp, making reliable distinction of HEP from CA challenging. Because the HEP and cardiac potentials are anatomically distinct, they may be separable via beamforming, a source localisation method that isolates brain activity at specific locations while suppressing external noise and interference. Here, the first known ground-truth validation of EEG beamforming for HEP source reconstruction was attempted, aiming to quantify source waveform recovery and spatial localisation accuracy using simulated EEG data. Using linearly constrained minimal variance (LCMV) beamforming, the following was investigated. (A) To test whether beamforming can recover a known signal, 128-channel EEG datasets were simulated for 3 models with a known HEP waveform: a single right insula (R-Ins) HEP (1), two temporally distinct HEPs in the R-Ins and right anterior cingulate cortex (R-ACC) (2), and two temporally overlapping HEPs in the same regions (3). Recovery was investigated by correlating the virtual electrode waveforms at the true location with the known true input waveform. (B) To test CA suppression, CA extracted from isoelectric EEG of brain-dead individuals providing CA with limited cortical activity, was integrated into the simulated EEG data. Source (-10 to -50dB) and sensor (0 to -30dB) signal-to-noise ratios (SNR) were systematically varied for each model with and without CA. (C) LCMV beamforming was then applied to retrospective empirical EEG data from hypertensive and anxiety individuals (n=106). Across simulations and empirical data, T-tests compared power in a HEP-dominated window to an earlier CA-dominated window. Null-space projection, using subject-specific QRS waveform and its temporal derivative, was applied to remove residual CA in reconstructed source waveforms. In model 1, beamforming achieved near-perfect recovery without CA (r>0.99, 0mm error) at source SNR of -30dB, remaining robust in the presence of CA (r=0.72-0.94, 0-5.7mm error). Recovery degraded at low SNR (<-20 dB; r<0.3, up to 27mm error). Models 2 and 3 showed similar patterns but introduced R-ACC to R-Ins leakage. Applied to empirical data, beamforming revealed significant HEP activity in the R-Ins and R-ACC across all pooled data in source space (p < 0.001). LCMV beamforming also revealed a significant HEP difference in the late R-ACC window (250-500 ms post R-peak) in hypertension versus controls (p = 0.040, d = 0.92) when poor SNR subjects were excluded. This effect strengthened after QRS cleaning (p = 0.035, d = 0.96). LCMV beamforming can reliably recover the simulated HEP while suppressing CA, provided source SNR is sufficiently high. Applied to empirical data, LCMV beamforming recovered HEP activity from interoceptive regions (R-Ins and R-ACC) and was sufficiently sensitive to detect clinically meaningful group differences. This study offers a source level approach to separate HEP activity from CA, a distinction that sensor-level analysis can struggle to make. Together, LCMV beamforming and scalp-based methods can provide converging evidence for genuine HEP activity.

---

## 论文详细总结（自动生成）

# 论文详细中文总结

## 1. 论文的核心问题与整体含义（研究动机和背景）

- **核心问题**：心跳诱发电位（HEP）是一种对心跳的皮层反应，被视为内感受的神经标志物，在临床研究中具有重要价值。然而，头皮记录的HEP严重受到心电伪迹（CA）的污染，传统头皮分析难以区分真实的HEP与CA。本文旨在验证是否可以通过波束成形（beamforming）这一源定位方法，利用HEP与CA在解剖上的不同，在源空间将二者有效分离。
- **整体含义**：提供一种可靠的源级工具，使研究者能够更准确地研究内感受的神经机制，避免CA的干扰，进而提升HEP在临床（如高血压、焦虑等）研究中的敏感性和特异性。

## 2. 论文提出的方法论：核心思想、关键技术细节

- **核心思想**：使用线性约束最小方差（LCMV）波束成形对128通道EEG进行源重建，利用空间滤波抑制来自心脏的远场伪迹，同时保留大脑内部HEP源的活动。通过加入空域投影（null-space projection）进一步去除重建源波形中的残余CA。
- **关键技术细节**：
  - **波束成形器**：LCMV波束成形，其权向量通过最小化输出方差同时保持对感兴趣源的无畸变响应来设计。
  - **源模型**：构建3个模拟模型：(1) 单一右脑岛（R-Ins）HEP源；(2) R-Ins与右前扣带回（R-ACC）两个时间上不同的HEP源；(3) 相同两个区域但时间上重叠的HEP源。
  - **CA集成**：从脑死亡个体的等电位EEG中提取实际CA（具有有限皮层活动），将其叠加到模拟EEG数据中。
  - **信噪比（SNR）控制**：系统变化源SNR（-10至-50 dB）和传感器SNR（0至-30 dB），测试不同噪声水平下的恢复表现。
  - **评估指标**：使用真实位置虚拟电极波形与已知真实输入波形的相关系数（r）和定位误差（mm）量化恢复精度；在经验数据中，通过T检验比较HEP主导窗口（晚窗）与CA主导窗口（早窗）的功率，并使用受试者特异性QRS波形及其时间导数进行零空间投影清理残余CA。
- **算法流程**（文字描述）：
  1. 生成模拟EEG数据：基于正向模型计算HEP源在头皮上的投影，叠加CA和传感器噪声。
  2. 计算数据协方差矩阵。
  3. 对每个体素构建LCMV空间滤波器，得到虚拟电极时间序列。
  4. 在已知真实源位置处提取虚拟电极波形，与输入波形计算相关系数。
  5. 对于经验数据：预处理EEG（滤波、剔除坏段），R峰对齐提取epoch；计算协方差；应用LCMV波束成形得到全脑源活动；定位感兴趣区域（R-Ins, R-ACC）的虚拟电极；进行CA零空间投影清理；统计检验（组内、组间）。

## 3. 实验设计：使用了哪些数据集 / 场景，对比了哪些方法

- **模拟数据**：
  - 基于标准大脑模型模拟128通道EEG，使用3种HEP源配置（单源、双源时序分离、双源重叠）。
  - 无CA和含CA两种条件，每种条件下变化源SNR和传感器SNR（多组组合）。
- **实证数据**：
  - 回顾性数据：来自高血压和焦虑个体的EEG记录（n=106），包含患者组和对照组。
  - 未使用其他对比方法（如ICA、回归等），仅验证LCMV波束成形本身的分离能力，但与传统头皮分析（文中提到传感器级分析难以区分）进行了定性对比。
- **Benchmark**：在模拟中，以已知真实输入波形作为ground truth，评估恢复精度；在实证中，无绝对基准，但通过检验HEP活动是否出现在预期脑区（右脑岛、前扣带回）以及组间差异是否具有临床意义来间接验证。

## 4. 资源与算力

- **文中未明确说明使用的GPU型号、数量或训练时长**。仅提及使用MATLAB环境下的FieldTrip工具箱进行波束成形分析，未提供具体计算资源信息。因此无法给出算力总结。

## 5. 实验数量与充分性

- **实验数量**：
  - 模拟实验：3种源模型 ×（无CA / 有CA）× 多个SNR水平（源SNR 5个水平，传感器SNR 4个水平，组合共20种条件），但文中仅报告了部分代表性结果（如模型1在不同SNR下的恢复指标表），未展示所有组合的完整矩阵，但已覆盖主要SNR范围。
  - 实证实验：对106名受试者进行全脑源定位，分别对R-Ins和R-ACC做HEP效应检验，并进一步根据SNR排除低质量受试者后比较高血压组与对照组。
- **充分性**：
  - 模拟实验系统变化了影响波束成形性能的关键参数（SNR），并使用了真实CA数据，设计较为严谨。
  - 实证数据样本量较大（n=106），但仅有单一数据集，缺乏独立验证集。
  - 未与其他CA去除方法（如ICA、SSP）进行直接对比消融实验，因此公平性有所欠缺。但本文的主要目标是验证LCMV波束成形本身能否分离HEP与CA，而非全面的方法比较。
- **客观性**：实验设计考虑了不同源模型（单一/双源）和时间重叠性，以及不同噪声水平，结果在模拟中给出了量化指标，较为客观。但在实证中，由于缺乏绝对真值，结论依赖统计显著性，存在一定局限。

## 6. 论文的主要结论与发现

- **模拟结果**：
  - 在无CA且源SNR≥-30 dB时，LCMV波束成形可实现近乎完美的恢复（r>0.99，0mm定位误差）。
  - 加入CA后，在高SNR下仍保持稳健（r=0.72-0.94，误差0-5.7mm）。
  - 当源SNR过低（低于-20 dB）时，恢复质量急剧下降（r<0.3，误差高达27mm）。
  - 双源模型（特别是时间重叠）会导致从R-ACC到R-Ins的泄漏（串扰），影响分离精度。
- **实证结果**：
  - 波束成形在源空间的所有汇集数据中检测到R-Ins和R-ACC的显著HEP活动（p < 0.001）。
  - 在排除低SNR受试者后，发现高血压组与对照组在R峰后250-500 ms的晚期窗口存在显著HEP差异（p = 0.040, d = 0.92）；经QRS零空间投影清理后效应增强（p = 0.035, d = 0.96）。
- **总体结论**：LCMV波束成形能够在足够高的信噪比下可靠分离HEP与CA，为内感受研究提供有效的源级工具，比传统头皮分析更具区分能力。

## 7. 优点

- **首次地面真实验证**：首次使用模拟数据系统评估LCMV波束成形在HEP源重建中的恢复精度和定位误差，提供了量化基准。
- **方法创新**：将波束成形与零空间投影结合，利用解剖先验分离HEP与CA，避免了传统盲源分离方法（如ICA）可能混合伪迹的问题。
- **实验设计系统**：模拟实验系统变化SNR，覆盖单源和双源、时间重叠等场景，实证数据样本量较大且包含临床分组对比。
- **结果可靠**：模拟和实证结果一致，验证了方法在足够SNR下的有效性，并发现低SNR会导致失效，为实际应用提供指导。

## 8. 不足与局限

- **方法局限性**：
  - 波束成形对SNR敏感，低SNR下恢复失败，要求数据质量较高（如HEP幅值足够大、噪声低）。
  - 双源模型显示存在源泄漏（串扰），尤其在时间重叠时，可能影响对邻近源的分离。
  - 仅测试了LCMV波束成形，未比较其他波束成形（如eigenspace beamforming）或不同协方差正则化策略。
- **实验覆盖不足**：
  - 模拟中仅使用单一真实CA模板，未考虑不同个体CA形态变异对结果的影响。
  - 实证数据仅来自高血压和焦虑人群，未在其他疾病或健康人群独立验证。
  - 未与常用的ICA去除CA方法进行定量比较，无法说明波束成形相对于现有方法的优势程度。
- **偏差风险**：
  - 实证数据分析中，排除低SNR受试者可能引入选择偏倚（排除标准基于信噪比，可能与临床特征相关）。
  - 未报告多重比较校正细节（如HEP效应检验是否进行了多重比较校正），可能增加假阳性风险。
- **应用限制**：
  - 需要高密度EEG（128通道）和准确的头部模型（MRI配准），限制了在临床快速场景中的推广应用。
  - 计算过程较复杂，对正则化参数（如协方差矩阵奇异值截断）的选择敏感，需专业知识调整。

（完）
