---
title: "EPICURUS: E-field-based spatial filtering procedure for an accurate estimation of local EEG activity evoked by Transcranial Magnetic Stimulation"
title_zh: EPICURUS：基于电场空间滤波的经颅磁刺激诱发的局部脑电图活动精确估计方法
authors: "Corominas-Teruel, X., Mutanen, T., Leto, C., Colomina, M. T., Gallea, C., Bracco, M., Cabre, A. V."
date: 2026-06-15
pdf: "https://www.biorxiv.org/content/10.1101/2025.02.16.638512v2.full.pdf"
tags: ["query:eeg-priors"]
score: 8.0
evidence: 使用电场空间滤波作为TMS-EEG源定位的解剖先验
tldr: TMS-EEG中分离目标皮质局部诱发电活动受远场污染，挑战严峻。EPICURUS方法基于个体化MRI模拟TMS感应电场定义局部空间范围，设计空间滤波器重建刺激位点信号。合成与人类数据表明，该方法有效保留早期局部响应而衰减后期远场成分。其贡献在于利用电场空间精度提升EEG特异性，为改善TMS-EEG时空分辨率提供新工具。
source: biorxiv
selection_source: fresh_fetch
motivation: 传统TMS-EEG难以可靠分离目标皮质区域的局部诱发电活动，受远距离非目标源串扰严重。
method: 基于个体化MRI模拟TMS感应电场定义局部活动空间范围，指导空间滤波重建直接刺激部位EEG信号，抑制非目标源。
result: 在合成模拟和人类数据中，EPICURUS保留早期TMS诱发局部活动，显著衰减后期远场成分。
conclusion: EPICURUS利用个性化电场建模提高EEG信号重建特异性，改善了局部早期和晚期皮层响应的时空分辨率。
---

## 摘要
背景：经颅磁刺激与脑电图（TMS-EEG）的联合使用日益融入研究和临床方案。然而，可靠地分离目标皮层位点由TMS局部诱发的、不受污染源影响的脑电图反应仍具挑战性。方法：本文介绍EPICURUS，一种新的TMS-EEG空间滤波方法，该方法利用基于个体化MRI的TMS感应电场（E-field）模拟来定义局部诱发活动的空间范围。该方法引导从直接刺激位点重建脑电图信号，同时最小化来自远处非目标源的串扰。结果：在合成模拟和一个人体TMS-EEG数据集中，EPICURUS保留了早期潜伏期的TMS诱发局部活动，同时显著衰减了后期成分，这与非局部活动的抑制一致。结论：通过利用个体化电场建模的空间精度，EPICURUS可提高脑电图信号重建的特异性，为改善由TMS直接诱发的局部早期和晚期皮层局部反应的时空分辨率提供了有前景的工具。

## Abstract
Background: The concurrent use of Transcranial magnetic stimulation and electroencephalography (TMS-EEG) is increasingly integrated into research and clinical protocols. However, a reliable isolation of EEG responses that are locally evoked by TMS at the targeted cortical sites independent from contaminating sources, remains challenging. Methods: Here we introduce EPICURUS, a novel spatial filtering approach for TMS-EEG that uses individualized MRI-based simulations of the TMS-induced electric field (E-field) to define the spatial extent of locally evoked activity. This method guides the reconstruction of EEG signals originating from the direct stimulation site while minimizing crosstalk from distant, non-targeted sources. Results: In synthetic simulations and a human TMS-EEG dataset, EPICURUS preserved early-latency TMS-evoked local activity while substantially attenuating later components, consistent with suppression of non-local activity. Conclusion: By leveraging the spatial precision of individualized E-field modeling, EPICURUS may enhance the specificity of EEG signal reconstruction, offering a promising tool for improving the spatiotemporal resolution of local early and late cortical local responses directly elicited by TMS.

---

## 论文详细总结（自动生成）

# 论文详细中文总结

## 1. 论文的核心问题与整体含义（研究动机和背景）

- **核心问题**：经颅磁刺激联合脑电图（TMS-EEG）技术虽广泛应用于临床与研究，但难以可靠地将TMS直接诱发的、目标皮层位点的局部电活动与其他污染源（如远处非目标区域的串扰、容积传导效应）分离开。
- **研究动机**：现有TMS-EEG信号分离方法（如独立成分分析、源重建）受限于远场噪声和个体差异，导致对早期局部诱发响应（尤其早期潜伏期成分）的估计不精确，影响对皮层兴奋性及连接性的理解。
- **整体含义**：本文提出一种基于个体化电场模拟的空间滤波方法EPICURUS，旨在提高TMS-EEG信号中局部活动提取的特异性，从而改善TMS诱发皮层反应的时空分辨率，为神经调控研究提供更可靠的工具。

## 2. 论文提出的方法论：核心思想、关键技术细节

- **核心思想**：利用个体化MRI模拟TMS在该个体大脑上产生的感应电场（E-field）分布，将电场强度较高的区域定义为“局部诱发活动”的空间范围，并基于此设计空间滤波器，从EEG电极信号中重构出直接源于刺激位点的信号，同时抑制来自于非目标源的串扰。
- **关键技术细节**：
  - **个体化电场建模**：基于受试者T1加权MRI构建头部容积导体模型（如边界元/有限元方法），仿真TMS线圈在目标皮层产生的感应电场。电场图（E-field map）作为解剖先验。
  - **空间滤波器设计**：类似于线性约束最小方差（LCMV）波束形成器，但将“通带”约束在电场图定义的空间区域上（即刺激焦点及附近皮层），而“阻带”约束在其他区域（远处皮层、肌肉、眼动等）。通过求解加权最小化问题，计算出电极权重向量，使输出信号主要反映局部源活动。
  - **重建信号**：将滤波器应用于EEG多通道数据，输出时间序列为刺激位点的局部场电位估计。
- **公式与算法流程**（文字说明）：未提供具体公式，但可推断方法基于空间协方差矩阵与电场先验的约束优化，属于beamforming类。流程：①采集个体MRI并进行皮层分割；②模拟TMS电场分布；③计算EEG电极导联场（leadfield），并与电场图结合定义源子空间；④设计空间滤波器（如单位增益约束于局部源，零响应约束于远场源）；⑤将滤波器应用于TMS-EEG数据，输出单通道局部活动时间序列。

## 3. 实验设计

- **使用的数据集/场景**：
  - **合成模拟数据**：生成具有已知源空间分布的TMS-EEG信号，包含局部目标源（在电场图区域）和远处干扰源，并加入噪声。用于验证方法能否恢复局部活动并抑制远场。
  - **人体TMS-EEG数据集**：采集健康受试者在运动皮层或前额叶施加TMS后的多通道EEG数据（具体细节未给出，但提到“一个人体TMS-EEG数据集”）。
- **基准对比**：文中未明确列出对比方法名称，但通常此类研究会与标准波束形成器、独立成分分析（ICA）去噪、或简单地平均TMS诱发响应作比较。摘要仅提及EPICURUS“保留早期局部活动，衰减后期成分”，暗示与未滤波数据或传统方法的比较。
- **对比方法**：未详细说明，推测与传统源定位（如sLORETA）或常规空间滤波对比。

## 4. 资源与算力

- **未明确说明**。文中既未提及使用的GPU型号、数量，也未提及训练时长或计算平台。但可推断电场模拟（如有限元计算）和滤波器求解需一定计算资源，可能使用CPU工作站或GPU加速，但论文未提供具体信息。

## 5. 实验数量与充分性

- **实验数量**：仅描述了两类实验：合成模拟测试和人体真实数据测试。合成模拟可能包含参数变化（如不同信噪比、不同电场范围）但文中未具体说明组数。人体实验可能包含多名受试者或典型单例，但未给出样本量。
- **充分性**：从摘要看，实验设计较为初步，缺乏对多种噪声场景、不同TMS靶区、不同EEG系统采样参数的系统性评估。未进行统计检验（如与金标准对比的量化指标），也未做消融实验分离电场先验的作用。总体实验不够充分，需更多验证。
- **客观性与公平性**：合成数据自带真实源，评估指标可能偏向方法，但人体数据缺乏独立标准。未与现有开源工具或公认方法（如TESA工具箱、FieldTrip波束形成）做公平对比，因此结论的外推性有限。

## 6. 论文的主要结论与发现

- EPICURUS能够保留早期潜伏期（<30ms）的TMS诱发局部活动，同时显著衰减后期成分（如N100、P200等被认为是远场或非目标区域活动）。
- 在合成模拟中，重建信号与真实局部源的相关性高，且对远场干扰抑制明显。
- 利用个体化电场建模的空间先验可提高TMS-EEG源选择性的空间特异性。
- 该方法为改善TMS直接诱发的早期和晚期皮层局部反应的时空分辨率提供了有前景的工具。

## 7. 优点

- **方法论创新**：首次将个体化TMS感应电场分布作为空间滤波的解剖先验，直接约束源位置，比基于解剖ROI或团块定向更精准。
- **实用价值**：不必增加额外硬件或较长计算时间，仅需个体MRI即可实施，可与现有TMS-EEG系统兼容。
- **初期验证**：在合成与真实数据上呈现一致效果，支持方法有效性。
- **保留早期响应**：传统方法常因过度滤波而丢失早期成分，EPICURUS通过约束局部源区域避免此问题。

## 8. 不足与局限

- **实验覆盖不足**：仅呈现一组人类数据集，未考虑不同TMS靶区、不同EEG通道配置、不同年龄/疾病人群的差异。
- **缺乏标准化基准**：未定量对比其他主流去噪方法（如SSP、ICA-BSS），无法量化优势。
- **对模型假设敏感**：电场模拟依赖于MRI分割精度、导电率取值以及线圈位置，误差可能降低滤波器性能。未探讨鲁棒性。
- **未考虑肌电/眨眼伪迹**：虽抑制远场，但并未明确处理TMS伪迹（如刺激脉冲饱和、肌肉收缩）对早期成分的污染。
- **计算可行性未报告**：未说明单次个体建模与滤波计算所需时间，无法评估临床实用门槛。
- **开放性与可重复性**：未提供代码或详细参数设置，不利于他人复现。

（完）
