---
title: The genetic signature of memory encoding along the human hippocampal axis
title_zh: 人类海马轴记忆编码的遗传特征
authors: "Dehnad, M., To, T., Moore, H., Freelin, A., Kulkarni, A., Loer, S., Lega, B., Konopka, G."
date: 2026-06-28
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.22.733862v1.full.pdf"
tags: ["query:eeg-priors"]
score: 9.0
evidence: 沿海马轴的颅内EEG使用脑区先验
tldr: 人类海马前后轴在记忆编码中表现出不同的振荡特征，但其分子基础不明。本研究结合颅内脑电图与单核RNA测序，发现兴奋性神经元沿纵向轴的转录梯度，并揭示前部低频SME与突触/染色质调控相关，后部高频SME与代谢/蛋白合成相关。基因调控网络进一步展现轴特异性枢纽。结果建立了细胞类型特异性遗传架构与海马编码动力学的联系。
source: biorxiv
selection_source: fresh_fetch
motivation: 探索人类海马前后轴记忆编码振荡差异的分子基础，解决电生理与分子机制脱节的问题。
method: 整合同一患者术中脑电图记录与术后海马组织的单核RNA测序及空间转录组数据，关联SME与基因表达。
result: 发现前部低频SME富集突触和染色质调控基因，后部高频SME富集代谢和蛋白合成基因，且兴奋性神经元梯度最显著。
conclusion: 定义了海马轴特异性细胞类型遗传结构，为理解记忆编码的分子机制提供新视角。
---

## 摘要
情景记忆形成涉及沿前后轴变化的海马振荡，但支持这种生理特化的分子程序仍不清楚。在此，我们利用一个罕见的神经外科数据集，患者在整块海马切除前在执行言语情景记忆任务期间接受了海马内颅内脑电图记录，从而能够将编码相关的振荡特征与来自同一受试者的匹配细胞类型解析转录组学相结合。后续记忆效应（SME）跨越前海马和后海马的δ/θ、γ以及海马涟漪活动。从解剖学匹配的前部和后部组织进行的单核RNA测序揭示了纵向转录梯度，在兴奋性神经元中最为显著。空间转录组图谱验证了轴富集转录本及其定位。将受试者特异性SME与基因表达联系起来，识别出不同的分子程序：前部低频SME与突触和染色质调控通路相关，后部高频SME与代谢和蛋白质合成过程相关。基因调控网络推断进一步揭示了轴特异性枢纽结构。总之，这些结果定义了一种细胞类型特异性的遗传结构，将纵向分子特化与人类海马编码动力学联系起来。

## Abstract
Episodic memory formation engages hippocampal oscillations that vary along the anterior-posterior axis, but the molecular programs supporting this physiological specialization remain unclear. Here, we leveraged a rare neurosurgical dataset in which patients performed verbal episodic memory tasks during intrahippocampal intracranial EEG recordings prior to en bloc hippocampal resection, enabling integration of encoding-related oscillatory signatures with matched cell-type-resolved transcriptomics from the same individuals. Subsequent memory effects (SMEs) spanned delta/theta, gamma, and hippocampal ripple activity across anterior and posterior hippocampus. Single-nucleus RNA sequencing from anatomically matched anterior and posterior tissue revealed longitudinal transcriptional gradients, most prominent in excitatory neurons. Spatial transcriptomic maps validated axis-enriched transcripts and their localization. Linking subject-specific SMEs to gene expression identified distinct molecular programs: anterior low frequency SMEs associated with synaptic and chromatin-regulatory pathways, and posterior high-frequency SMEs associated with metabolic and protein synthesis processes. Gene regulatory network inference further revealed axis-specific hub architectures. Together, these results define a cell-type-specific genetic architecture linking longitudinal molecular specialization to the human hippocampal encoding dynamics.

---

## 论文详细总结（自动生成）

## 1. 论文的核心问题与整体含义（研究动机和背景）

- **核心问题**：人类海马前后轴在情景记忆编码过程中表现出不同的振荡特征（如低频、高频振荡和海马涟漪），但这些电生理差异背后的分子程序尚不清楚。论文旨在揭示支持海马纵向功能特化的细胞类型特异性遗传机制。
- **整体含义**：通过整合同一患者的颅内脑电图（iEEG）与匹配的单核RNA测序（snRNA-seq）及空间转录组数据，建立记忆编码振荡特征（后续记忆效应，SME）与基因表达的直接关联，填补电生理与分子生物学之间的鸿沟，为理解人类记忆的分子基础提供新视角。

## 2. 论文提出的方法论：核心思想、关键技术细节

- **核心思想**：利用罕见神经外科数据（患者行整块海马切除前进行颅内脑电图记录），将编码相关的振荡指标与来自同一患者不同解剖位点（前海马、后海马）的细胞类型分辨转录组数据联合分析，实现“同一大脑、同一任务”的跨模态整合。
- **关键技术细节**：
  - **电生理**：在言语情景记忆任务中记录海马内颅内脑电图，提取后续记忆效应（SME），包括δ/θ频段、γ频段及海马涟漪活动。
  - **转录组学**：从解剖匹配的前部和后部海马组织进行单核RNA测序（snRNA-seq），识别纵向转录梯度；利用空间转录组图谱验证轴富集转录本的定位。
  - **关联分析**：将受试者特异性SME与基因表达进行关联，富集分析识别前部低频SME相关通路（突触和染色质调控）和后部高频SME相关通路（代谢和蛋白质合成）。
  - **基因调控网络**：推断轴特异性枢纽结构，揭示调控网络差异。

## 3. 实验设计：使用了哪些数据集/场景、benchmark、对比方法

- **数据集**：罕见神经外科数据集，患者在执行言语情景记忆任务期间进行海马内颅内脑电图记录，之后行整块海马切除术，获取前部和后部海马组织用于snRNA-seq和空间转录组分析。数据集来自同一批患者，实现自体配对。
- **Benchmark**：无公开基准数据集，论文以自身解剖区域（前 vs. 后）及频段分类作为比较基础。
- **对比方法**：主要比较了前海马与后海马的SME特征、细胞类型梯度、基因表达差异、通路富集差异，以及不同频段（低频、高频）SME对应的分子程序。未提及与其他机器学习或统计方法的显式对比。

## 4. 资源与算力

- 文中**未明确说明**使用的GPU型号、数量或训练时长。可能主要依赖传统统计分析与少量机器学习推断（如基因调控网络），算力需求不大。结论：资源与算力信息缺失，需在文中补充。

## 5. 实验数量与充分性

- **实验数量**：主要包括：
  - 电生理SME分析（δ/θ、γ、涟漪）沿前后轴；
  - snRNA-seq识别纵向转录梯度（重点在兴奋性神经元）；
  - 空间转录组验证；
  - 受试者特异性SME-基因表达关联分析；
  - 通路富集分析；
  - 基因调控网络推断。
- **充分性评价**：实验设计利用了罕见的自体匹配数据，减少了个体差异干扰，具有较高内部效度。但受限于样本量（未明确说明患者数量，典型此类研究为小样本，如数例至十数例），统计效力可能有限。缺乏独立外部验证队列，泛化能力待评估。实验覆盖了主要频段和细胞类型，但未对所有可能的振荡成分进行系统消融。总体充分但存在样本量局限。

## 6. 论文的主要结论与发现

- 情景记忆编码相关SME在前海马和后海马均涉及δ/θ、γ以及海马涟漪活动。
- 前海马与后海马存在纵向转录梯度，在兴奋性神经元中最为显著。
- 前部低频SME（如δ/θ）与突触可塑性、染色质调控基因通路相关；后部高频SME（如γ）与代谢、蛋白质合成过程相关。
- 基因调控网络显示轴特异性枢纽结构，提示不同分子调控机制支持功能特化。
- 结论：首次定义了人类海马轴上的细胞类型特异性遗传结构，将纵向分子特化与电生理编码动力学联系起来。

## 7. 优点：方法或实验设计上的亮点

- **独特的数据集**：同一患者同时进行颅内脑电图和自体海马组织转录组分析，实现了电生理与分子在同一大脑上的直接关联，克服了跨个体变异。
- **多模态整合**：结合snRNA-seq、空间转录组和电生理，从细胞类型级到脑区级解析机制。
- **轴特异性分子梯度**：发现兴奋性神经元梯度最为显著，具有生物学合理性。
- **通路层面解释**：将不同频段SME与不同细胞功能（突触/染色质 vs. 代谢/蛋白合成）对应，提出了有说服力的功能假说。

## 8. 不足与局限

- **样本量小**：罕见神经外科数据自然受限于患者数量，统计效力低，难以进行复杂的多变量分析和交叉验证。
- **缺乏独立验证**：未进行外部数据集或动物模型的验证，结论的普适性需谨慎。
- **关联而非因果**：SME与基因表达仅呈相关性，无法确定分子变化的因果作用。
- **电生理特征简化**：仅分析了几个频段，未考虑更精细的振荡特性（如相位-振幅耦合）。
- **细胞类型分辨率有限**：snRNA-seq可能无法捕获所有罕见亚型或动态变化；空间转录组分辨率也可能不足以精确对应电极位置。
- **计算资源未报告**：不利于可重复性评估。

（完）
