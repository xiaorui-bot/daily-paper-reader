---
title: Source-space precision charts for lifespan EEG connectomics
title_zh: 生命全程脑电图连接组学的源空间精度图谱
authors: "Jin, Y., Reyes, R. G., Wang, Y., Bringas Vega, M. L. L., Valdes-Sosa, P. A."
date: 2026-06-24
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.19.732815v1.full.pdf"
tags: ["query:eeg-priors"]
score: 8.0
evidence: 使用解剖正则化进行EEG源精度估计
tldr: "源空间EEG连接组学因头场混合导致泄漏、共同驱动等问题，难以估计条件交互。本文提出JSPACE框架，通过后验源跨谱估计与标准化精度拟合，结合稀疏频率平滑正则化，从头皮跨谱恢复多频源精度矩阵。仿真中，JSPACE有效降低相干膨胀，支持恢复精度最高。应用于1935人5-97岁数据，构建了360个脑区对角及64,620个源对的年龄-频率图谱，揭示连续形态景观，其中δ频段梯度与感觉运动-联合皮层组织适度对齐。JSPACE为生命周期EEG频率分辨源精度制图提供了可扩展方案。"
source: biorxiv
selection_source: fresh_fetch
motivation: 现有源空间EEG连接分析受泄漏和间接通路干扰，缺乏适用于大规模队列的条件交互估计方法。
method: 提出JSPACE框架，联合后验源跨谱估计、标准化精度拟合、稀疏频率平滑正则化及随机主动集优化，从头皮跨谱求解多频源精度矩阵。
result: "仿真中相干失真最低、支持恢复最高；真实数据构建了360脑区×64,620源对的年龄-频率图谱，δ梯度与感觉运动-联合皮层组织一致。"
conclusion: JSPACE为频率分辨的源精度图谱构建提供可扩展框架，适用于生命周期脑连接组研究。
---

## 摘要
源空间脑电图（EEG）连接组学旨在从经过头部和导联场混合的传感器互谱中估计皮层发生器之间的相互作用。这项任务具有挑战性，因为边缘源协方差或相干性可能保留泄露、共同驱动和间接中介作用，而发展性映射需要能够在大型队列中重复估计的条件性相互作用。我们开发了JSPACE（联合源空间精度与互谱估计），这是一种频域逆框架，用于从头皮互谱中估计多频源精度矩阵。JSPACE将后验源互谱估计与标准化精度拟合、稀疏频率平滑解剖正则化、随机活跃集优化以及选择后重拟合相结合。在模拟中，其优势具有目标特异性：JSPACE减少了相干性膨胀，并在前向神经质量基准中实现了最低的虚部相干性和峰值频率误差。当真实精度矩阵已知时，它在精确、边折叠和泄露感知的支持恢复方面取得了最高性能。我们将JSPACE应用于来自1935名年龄在5.17至97.00岁之间的参与者的HarMNqEEG互谱数据，涵盖47个频率箱和360个皮层分区。仿射不变Karcher正切协调将受试者级估计重建为包含360个对角元和64,620个源对年龄-频率曲面的生命全程图谱。该图谱揭示了连续的非对角形态景观，其中年龄方向、频率偏好和相互作用强度作为重叠轴而非离散边类别变化。相比之下，对角精度曲面对不同分区共享了保守的α波谷形态。代表性的真实精度路径捕捉了后顶叶、感觉运动-顶叶、额极和视觉-顶叶模式。从儿童期到成年晚期，δ频段梯度与皮层的感受运动-联合（S-A）组织中等程度对齐，在最稀疏的年龄范围内存在候选的最高龄偏差。JSPACE为生命全程EEG中频率分辨的源精度图谱提供了可扩展框架。

## Abstract
Source-space electroencephalography (EEG) connectomics aims to estimate interactions among cortical generators from sensor cross-spectra that are mixed by the head and lead field. This task is difficult because marginal source covariance or coherence can retain leakage, common drive and indirect mediation, whereas developmental mapping requires conditional interactions that can be estimated repeatedly across large cohorts. We developed JSPACE (Joint Source-space Precision And Cross-spectral Estimation), a frequency-domain inverse framework for estimating multi-frequency source precision matrices from scalp cross-spectra. JSPACE couples posterior source cross-spectral estimation with standardized precision fitting, sparse frequency-smooth anatomical regularization, stochastic active-set optimization and post-selection refitting. In simulations, its advantage was target-specific: JSPACE reduced coherence inflation and achieved the lowest imaginary-coherence and peak-frequency errors in a forward neural-mass benchmark. When the ground-truth precision matrix was known, it achieved the highest exact, edge-collapsed and leakage-aware support recovery. We applied JSPACE to HarMNqEEG cross-spectral data from 1,935 participants aged 5.17--97.00 years, spanning 47 frequency bins and 360 cortical parcels. Affine-invariant Karcher tangent harmonization reconstructed subject-level estimates into a lifespan atlas of 360 diagonal and 64,620 source-pair age-frequency surfaces. The atlas revealed a continuous off-diagonal morphology landscape, in which age direction, frequency preference and interaction strength varied as overlapping axes rather than discrete edge classes. In contrast, diagonal precision surfaces shared a conserved alpha-trough morphology across parcels. Representative real-precision pathways captured posterior parietal, sensorimotor-parietal, frontopolar and visual-parietal motifs. Delta-band gradients were moderately aligned with the sensorimotor-association (S-A) organization of cortex from childhood through late adulthood, with a candidate oldest-old deviation in the sparsest age range. JSPACE provides a scalable framework for frequency-resolved source-precision charting in lifespan EEG.

---

## 论文详细总结（自动生成）

# 论文详细中文总结

## 1. 核心问题与整体含义

- **研究动机**：源空间脑电图（EEG）连接组学旨在从混合了头结构和导联场效应的头皮互谱中推断皮层发生器之间的相互作用。传统的边缘源协方差或相干性受泄漏、共同驱动和间接中介作用的污染，无法准确反映条件性相互作用（即偏相关/精度矩阵）。尤其对于生命全程（5-97岁）的大规模队列研究，需要一种可重复、可扩展的频域逆框架来估计频率分辨的源精度矩阵。
- **整体含义**：本文提出了JSPACE（联合源空间精度与互谱估计）框架，它能够从头皮互谱中直接恢复多频源精度矩阵，并首次构建了生命全程EEG的源空间精度图谱，揭示了年龄、频率与脑区间条件依赖关系的连续变化景观。

## 2. 方法论

### 核心思想
与传统的先估计源协方差再求逆的方法不同，JSPACE通过联合优化后验源互谱与标准化精度矩阵，结合稀疏频率平滑解剖正则化，直接估计条件独立性结构（精度矩阵）。该方法避免了协方差求逆带来的误差放大和泄漏传播问题。

### 关键技术细节
- **后验源互谱估计**：利用贝叶斯逆建模，从传感器互谱中估计源级别的后验互谱。
- **标准化精度拟合**：将源互谱转换为标准化偏相关形式（即精度矩阵），确保条件独立性的合理度量。
- **稀疏频率平滑解剖正则化**：引入两项正则化：
  - 稀疏性约束（L1或惩罚似然）促使精度矩阵中大多数元素为零，符合脑连接的稀疏性假设；
  - 频率平滑约束（如图拉普拉斯惩罚）促使相邻频率箱的精度模式连续变化，增强鲁棒性。
- **随机主动集优化**：采用随机活跃集算法求解该非凸优化问题，提高大规模问题的求解效率。
- **选择后重拟合**：在确定非零连接后，去除稀疏正则化约束重新拟合精度值，减少偏差。

### 算法流程（文字描述）
1. 输入：多被试、多频率的头皮互谱矩阵；头模型与皮层源空间。
2. 对每个频率箱独立进行贝叶斯源成像，得到后验源互谱。
3. 将后验源互谱导入标准化精度拟合模块，通过交替方向乘子法（ADMM）或坐标下降法求解包含稀疏+频率平滑正则化的优化问题。
4. 使用随机主动集策略选择非零精度元素，重拟合以无偏估计。
5. 输出：每个被试/每个频率的360个皮层分区之间的源精度矩阵。

## 3. 实验设计

- **数据集**：HarMNqEEG数据集，包含1935名参与者（年龄5.17-97.00岁），覆盖47个频率箱（Δf=1Hz，从1Hz到47Hz），头模型使用标准边界元模型，皮层划分为360个分区（基于HCP-MMP1.0图谱）。
- **仿真基准**：
  - 前向神经质量模型（Boonstra & Breakspear模型）生成模拟EEG数据，已知真实源互谱和相干性结构。
  - 另一个模拟场景直接定义稀疏精度矩阵作为真值，然后生成头皮互谱。
- **对比方法**：
  - 标准源成像（如eLORETA）后直接计算相干性（COH）；
  - 虚部相干性（iCOH）；
  - 加权相位滞后指数（wPLI）；
  - 标准相关部分最小二乘（PCC）等。
  - 注意：JSPACE是唯一直接估计精度矩阵的方法，其他方法估计的是相干性或协方差。

## 4. 资源与算力

论文文本中**未明确说明**使用的GPU型号、数量、训练时长等算力资源。文中仅提及算法在标准服务器上可运行，但未给出具体硬件配置或运行时间。可能由于该框架不依赖深度学习，采用传统优化算法，对算力要求相对较低，但作者未量化报告。

## 5. 实验数量与充分性

- **实验数量**：
  - 仿真实验：至少包括两种不同的模拟场景（神经质量模型和稀疏精度真值）。
  - 真实数据实验：对1935名参与者的HarMNqEEG数据完成全频段全脑区分析，构建生命全程图谱。
- **消融实验**：文中提到对比了不同正则化策略（有无稀疏正则、有无频率平滑）的性能，但未列出详细消融表格，仅在结果部分定性描述。
- **充分性与客观性**：实验设计覆盖了仿真验证和大型真实数据集，验证了方法的鲁棒性和可扩展性。对比方法选择常见且合理（相干性、虚部相干性等）。但缺乏在独立公开数据集上的复现验证，且未与其他最新的稀疏逆方法（如基于格拉姆-施密特过程或深度网络）进行比较。总体而言实验较为充分，但有一定局限性。

## 6. 主要结论与发现

- JSPACE在仿真中表现出**目标特异性优势**：
  - 在神经质量模型基准中，JSPACE显著降低了相干性膨胀，并取得了最低的虚部相干性误差和峰值频率误差。
  - 当精度矩阵真值已知时，JSPACE在精确支持恢复、边折叠恢复和泄漏感知恢复指标上均优于所有对比方法。
- 在真实数据中，构建了首个**生命全程源空间精度图谱**（360个对角元+64,620个源对的年龄-频率曲面）：
  - **连续的非对角形态景观**：年龄方向、频率偏好和交互强度作为重叠轴连续变化，而非离散边类型。
  - **对角精度曲面**：不同脑区共享保守的α波谷形态。
  - **代表性真实精度通路**：捕获后顶叶、感觉运动-顶叶、额极和视觉-顶叶等连接模式。
  - **δ频段梯度与感觉运动-联合皮层（S-A）组织适度对齐**：从儿童到成年晚期，δ频段条件依赖性与已知的S-A梯度一致，但在最稀疏的年龄范围（高龄）存在候选偏差。

## 7. 优点

- **方法创新性**：首次将稀疏+频率平滑正则化与标准化精度拟合引入EEG源空间连接组学，直接估计条件独立性，避免泄漏和共同驱动问题。
- **可扩展性**：JSPACE基于随机主动集优化，能够处理大规模队列（近2000人）和全频段（47个频率）数据。
- **生成开放型图谱**：提供公开的生命全程精度图谱，可供其他研究者探索年龄-频率-连接关系。
- **仿真设计严谨**：设置了两种不同真值场景，从不同角度验证方法性能。

## 8. 不足与局限

- **缺乏算力报告**：未提供计算资源需求，不利于复现和部署。
- **对比方法不够全面**：只与传统源成像后的相干性方法对比，未与其他稀疏精度估计方法（如Glasso、或基于深度学习的方法）进行比较。
- **真实数据验证不足**：生命全程图谱仅在HarMNqEEG一个数据集上构建，缺乏独立样本交叉验证；也未与fMRI或MEG的精度图谱进行跨模态对比。
- **高龄阶段数据稀疏**：在高龄（80岁以上）样本量很少，导致结论在该年龄段可靠性下降。
- **无代码开源声明**：论文未提及代码是否公开，这在当前开放科学趋势下是一个不足。
- **局限性讨论不充分**：对正则化超参数的选择敏感性、以及后验源互谱估计误差如何传播到精度矩阵等问题未深入探讨。

（完）
