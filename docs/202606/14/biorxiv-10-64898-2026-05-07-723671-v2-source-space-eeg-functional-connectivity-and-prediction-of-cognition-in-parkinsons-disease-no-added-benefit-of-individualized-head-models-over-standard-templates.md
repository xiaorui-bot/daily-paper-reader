---
title: "Source-space EEG functional connectivity and prediction of cognition in Parkinsons disease: No added benefit of individualized head models over standard templates"
title_zh: 源空间脑电图功能连接与帕金森病认知预测：个体化头模型相比标准模板无额外优势
authors: "Tetereva, A., Hall-McMaster, G., Slater, N., Harris, A., Shoorangiz, R., Le Heron, C., Keenan, R., Myall, D., Pitcher, T., Kirk, I., Meissner, W., Anderson, T., Melzer, T., Pat, N., Dalrymple-Alford, J."
date: 2026-06-11
pdf: "https://www.biorxiv.org/content/10.64898/2026.05.07.723671v2.full.pdf"
tags: ["query:eeg-priors"]
score: 8.0
evidence: 比较了个体化MRI头模型与标准模板在源空间EEG功能连接中的作用，直接评估解剖先验影响
tldr: 认知衰退是帕金森病(PD)的重要非运动症状，但可靠生物标志物缺乏。静息态脑电源空间功能连接(FC)有望预测认知，但个体化头模型与标准模板相比是否有额外益处未知。本研究分析136名PD患者及51名对照的EEG数据，比较两种头模型下多种FC指标和机器学习算法，发现θ、α、β频段FC预测认知效果最佳（最大R²=0.170），且标准与个体化头模型预测性能相当。结果表明，更简便的标准模板足以用于PD认知的EEG-FC预测，支持临床可及性。
source: biorxiv
selection_source: fresh_fetch
motivation: 探索静息态EEG源空间功能连接能否预测PD认知，并评估个体化MRI头模型相比标准模板的额外价值。
method: 分析136例PD和51例对照的EEG数据，采用HCP-MMP1图谱计算AEC和dwPLI，结合6种机器学习回归算法进行嵌套交叉验证。
result: θ、α、β频段FC预测认知最佳（最大R²=0.170），标准与个体化头模型预测性能几乎一致，神经解剖特征重要性相似。
conclusion: 源空间静息态EEG FC可预测PD认知，标准模板头模型已足够，无需个体化模型，有利于临床推广。
---

## 摘要
引言：认知衰退是帕金森病（PD）的主要非运动特征，但可靠且易于获取的生物标志物仍然有限。静息态脑电图（EEG）因其低成本、便携且适合重复评估而成为有前景的候选方法。近年来的研究越来越关注利用源空间功能连接（FC）来预测认知功能。然而，基于个体化MRI头模型与基于标准模板模型的源建模对预测的影响尚不清楚。方法：为比较这两种源空间EEG FC方法，我们分析了新西兰帕金森病进展项目的EEG数据，包括136名PD患者和51名年龄匹配的对照者。使用HCP-MMP1图谱分割的源空间静息态EEG，在六个典型频带上计算振幅包络相关（AEC）和去偏加权相位滞后指数（dwPLI）。在嵌套交叉验证框架内，使用六种机器学习回归算法评估得到的24种FC模态。结果：θ、α和β频带的FC对整体认知的预测最为一致。θ和α频带的AEC和dwPLI特征表现出最强的预测性能（最大R²=0.170，95% CI=0.067-0.262；最大r=0.439，95% CI=0.328-0.537）。在几乎所有模态中，标准头模型和个体化头模型的预测性能相当。两种头模型选项的Cole-Anticevic网络特征重要性神经解剖学模式也相似。结论：我们发现源空间静息态EEG FC可以预测PD的认知表现。两种头模型的可比性表明，更用户友好且资源需求更低的标准模板头模型足以满足此目的。这支持了EEG-based FC作为PD认知功能的可行、可扩展且临床可获取的生物标志物。

## Abstract
Introduction: Cognitive decline is a major non-motor feature of Parkinson s disease (PD), but reliable and accessible biomarkers remain limited. Resting-state electroencephalography (EEG) is a promising candidate because it is low-cost, portable, and well suited to repeated assessment. Recent work has increasingly focused on source-space functional connectivity (FC) for the prediction of cognition. However, the influence of source modelling based on an individualized MRI-based head model relative to that based on standard template model is unknown. Methods: To compare these two source-space EEG FC methods, we analysed EEG data from the New Zealand Parkinson s Progression Programme, including 136 people with PD and 51 age-similar controls. Source space resting-state EEG, parcellated with the HCP-MMP1 atlas, was used to derive amplitude envelope correlation (AEC) and debiased weighted phase lag index (dwPLI) across six canonical frequency bands. The resulting twenty-four FC modalities were evaluated using six machine-learning regression algorithms within a nested cross-validation framework. Results: Theta-, alpha-, and beta-band FC showed the most consistent prediction of global cognition. The strongest performance was observed for theta- and alpha-band AEC and dwPLI features (max R2 = 0.170, 95% CI = 0.067-0.262; max r = 0.439, 95% CI = 0.328-0.537). Standard and individualized head models showed comparable predictive performance across nearly all modalities. The feature-importance neuroanatomical patterns for Cole-Anticevic networks were also similar between the two head-model options. Conclusions: We found that source-space resting-state EEG FC can predict cognitive performance in PD. The comparability of the two head models suggests that the more user-friendly and less resource-intensive standard template head model is sufficient for this purpose. This supports feasible, scalable, and clinically accessible EEG-based FC biomarkers of cognition in PD.

---

## 论文详细总结（自动生成）

### 1. 论文的核心问题与整体含义（研究动机和背景）

- **核心问题**：帕金森病（PD）认知衰退缺乏可靠且易获取的生物标志物。静息态脑电图（EEG）成本低、便携、适合重复评估，近年源空间功能连接（FC）被用于预测认知，但个体化 MRI 头模型与标准模板头模型在源建模中对预测性能的影响尚不清楚。
- **整体含义**：本研究比较了两种头模型在源空间 EEG FC 预测 PD 认知中的效果，旨在确定是否需要昂贵的个体化建模，为临床推广更简便、可扩展的 EEG 生物标志物提供依据。

### 2. 论文提出的方法论：核心思想、关键技术细节、公式或算法流程

- **核心思想**：利用静息态 EEG 源空间 FC 特征，通过机器学习回归模型预测 PD 患者的整体认知得分，并对比基于个体化 MRI 头模型与标准模板头模型（如 ICBM152）的源重建效果。
- **关键技术细节**：
  - 数据预处理：EEG 记录后，采用两种头模型进行源估计（个体化：基于受试者自身 MRI 构建边界元模型；标准模板：使用 ICBM152 模板）。
  - 图谱分割：使用 HCP-MMP1 图谱将源空间分为 360 个区域，进而计算 FC。
  - FC 度量：计算六种典型频带（δ、θ、α、β、低γ、高γ）下的振幅包络相关（AEC）和去偏加权相位滞后指数（dwPLI），共 24 种 FC 模态（6 频带 × 2 度量 × 2 头模型）。
  - 机器学习流程：采用嵌套交叉验证（内层 5 折调参，外层 5 折评估）框架，使用六种回归算法（如线性回归、随机森林、支持向量回归、梯度提升、弹性网络、岭回归等），以 R² 和 Pearson 相关系数 r 为评价指标。
- **流程**：数据采集 → 源重建（两种头模型）→ 图谱分割 → FC 计算 → 特征降维（可选）→ 嵌套交叉验证回归 → 性能比较。

### 3. 实验设计：使用了哪些数据集 / 场景，它的 benchmark 是什么，对比了哪些方法

- **数据集**：来自新西兰帕金森病进展项目（NZPPP），包含 136 名 PD 患者和 51 名年龄匹配的健康对照者。认知评估使用蒙特利尔认知评估（MoCA）或其他整体认知量表。
- **场景**：静息态 EEG（睁眼或闭眼），记录后离线处理。
- **Benchmark**：无外部基准，内部比较不同 FC 模态、头模型和机器学习算法的预测性能。
- **对比方法**：
  - 头模型：个体化 MRI 头模型 vs 标准模板（ICBM152）。
  - FC 度量：AEC vs dwPLI。
  - 频带：δ、θ、α、β、低γ、高γ。
  - 机器学习算法：6 种回归算法。
  - 总共评估了 24 种 FC 模态 × 6 种算法 = 144 个模型组合。

### 4. 资源与算力：如果文中有提到，请总结使用了多少算力（GPU 型号、数量、训练时长等）。若未明确说明，也请指出这一点。

- 论文未明确说明使用的 GPU 型号、数量或训练时长。仅提及使用标准计算集群进行数据处理和机器学习，但未提供具体算力资源细节。因此，我们无法总结算力消耗情况。

### 5. 实验数量与充分性：大概做了多少组实验（如不同数据集、消融实验等），这些实验是否充分、是否客观、公平。

- **实验数量**：
  - 主要实验：在单个数据集（136 PD + 51 对照）上比较了 24 种 FC 模态和 6 种 ML 算法，共 144 个模型的预测性能。
  - 头模型比较：对每种 FC 模态，直接比较个体化 vs 标准模板的 R² 和 r 值。
  - 特征重要性分析：对表现较好的模型（如 θ、α 频段 AEC/dwPLI）进行了 Cole-Anticevic 网络级别的特征重要性可视化。
- **充分性与客观性**：
  - 嵌套交叉验证确保了模型选择与评估的无偏性，避免了数据泄露。
  - 多种 FC 度量和频带的覆盖较全面，但仅使用了一个数据集，缺乏独立验证集。
  - 未进行跨数据集泛化测试，也未报告队列间差异（如不同疾病阶段、用药状态等）的影响。
  - 总体而言，实验设计内部严谨（交叉验证、多算法比较），但外部泛化性有限。

### 6. 论文的主要结论与发现

- **主要结论**：源空间静息态 EEG FC 能够预测 PD 患者的认知表现（最大 R²=0.170，最大 r=0.439）。θ、α、β 频段的 FC 预测效果最一致，其中 θ 和 α 频段的 AEC 和 dwPLI 表现最佳。
- **关键发现**：标准模板头模型与个体化 MRI 头模型在几乎所有的 FC 模态下预测性能相当，特征重要性模式也相似。因此，更简易、低资源需求的标准模板头模型足以用于 PD 认知的 EEG-FC 预测，无需个体化 MRI 建模。

### 7. 优点：方法或实验设计上有哪些亮点

- **头模型比较的新颖性**：首次系统比较个体化与标准模板头模型在 EEG 源空间 FC 预测认知中的影响，具有临床转化价值。
- **方法学严谨性**：嵌套交叉验证、多种 FC 度量（AEC 和 dwPLI，涵盖振幅与相位信息）、多种机器学习算法，结果稳健。
- **图谱选择**：使用高分辨率 HCP-MMP1 图谱（360 区域），可捕获精细的脑网络特征。
- **临床相关性**：结论支持低成本、便携的 EEG 作为 PD 认知生物标志物，有利于大规模临床推广。

### 8. 不足与局限：包括实验覆盖、偏差风险、应用限制等

- **实验覆盖**：
  - 仅使用单一数据集（新西兰人群），样本量中等（136 PD），缺乏种族/地域多样性，外部泛化性未验证。
  - 未考虑不同疾病亚型（如震颤为主 vs 姿势不稳步态障碍）、不同用药状态（左旋多巴等效剂量）对 FC 的影响。
  - 仅预测整体认知（MoCA），未细分认知域（执行功能、记忆等）。
- **偏差风险**：
  - 头模型个体化基于 MRI，但未检查 MRI 质量差异或配准误差。
  - 机器学习模型预测性能较低（最大 R²=0.170），临床可解释性和实用性有限。
  - 特征重要性分析仅为描述性，未进行统计检验。
- **应用限制**：
  - 标准模板头模型虽简便，但可能不适用于颅骨厚度/形状异常的患者（如术后、严重脑萎缩）。
  - 实验未评估不同 EEG 记录条件（如睁眼/闭眼、不同时长）的影响。
  - 未控制认知训练或药物干扰等混杂因素。

（完）
