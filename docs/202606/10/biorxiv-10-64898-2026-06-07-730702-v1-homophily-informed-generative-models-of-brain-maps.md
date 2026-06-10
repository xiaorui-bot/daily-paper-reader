---
title: Homophily-informed generative models of brain maps
title_zh: 基于同质性的脑图谱生成模型
authors: "Bazinet, V., Liu, Z.-Q., Milisav, F., Luppi, A. I., Misic, B."
date: 2026-06-08
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.07.730702v1.full.pdf"
tags: ["query:eeg-priors"]
score: 6.0
evidence: 利用区域间同质性建模脑图，为EEG分析提供解剖先验
tldr: 大脑的多尺度脑图成因不明。本文基于区域间同质性提出生成模型，评估六种定义和43个经验脑图，发现同质性足以重建多数脑图，生物相似性和功能连接贡献常超过几何距离；低同质性脑图存在未解释变异，揭示规范关系未捕获的皮层组织轴。该模型能解缠脑特征间复杂关系并推断其整合，突出同质性对脑图布局的基础贡献。
source: biorxiv
selection_source: fresh_fetch
motivation: 探究塑造多尺度脑图空间模式的基本驱动力，即区域间在物理、分子或功能空间中的同质性。
method: 定义六种区域间同质性（物理邻近、结构/功能连接、层状/受体/转录相似性），构建生成模型并基于43个经验脑图验证。
result: 同质性可准确重建多数脑图，生物相似性和功能连接贡献常超几何距离；低同质性脑图存在一致未解释变异。
conclusion: 同质性生成模型可解缠脑特征间复杂关系并推断整合，揭示同质性对脑生物特征拓扑布局的基础作用。
---

## 摘要
大脑的结构和功能组织可以在多个尺度上进行研究，从而产生生物特征的详尽地形脑图谱。是什么潜在力量塑造了它们的空间模式？这里我们引入了一个基于区域间同质性概念的多尺度脑图谱简单生成模型：即在给定的物理、分子或功能空间中邻近的区域倾向于显示相似的生物特征。我们根据六种区域间同质性的定义评估了该模型，包括物理邻近性、结构和功能连接性，以及层状、受体和转录相似性，并跨越了使用多种成像、电生理学和组织学技术估计的43个经验脑图谱。我们表明，同质性原则足以精确重建许多图谱，其中生物相似性和功能连接性通常比大脑几何结构贡献更大。我们还识别了低同质性图谱中一致性的无法解释变异模式，揭示了未被典型区域间关系捕获的皮层组织轴。最后，我们表明基于同质性的生成模型可用于解开脑特征之间的复杂关系，并对它们如何组合在一起做出新的推断。总的来说，这项工作强调了同质性对大脑众多生物特征地形布局的基础性贡献。

## Abstract
The structural and functional organization of the brain can be studied across multiple scales, yielding richly detailed topographic brain maps of biological features. What are the underlying forces that shape their spatial patterning? Here we introduce a simple generative model of multiscale brain maps based on the concept of inter-regional homophily: the tendency for regions that are proximal in a given physical, molecular or functional space to display similar biological features. We evaluate the model with respect to six definitions of inter-regional homophily, including physical proximity, structural and functional connectivity, and laminar, receptor and transcriptional similarity, and across 43 empirical brain maps estimated using multiple imaging, electrophysiological and histological technologies. We show that homophilic principles are sufficient to accurately reconstruct many maps, with biological similarity and functional connectivity often contributing more than the brain's geometry. We also identify consistent patterns of unexplained variation in maps with low homophily, revealing axes of cortical organization not captured by canonical inter-regional relationships. Finally, we show that homophily-informed generative models can be used to disentangle complex relationships between brain features and make new inferences on how they fit together. Collectively, this work highlights the fundamental contribution of homophily to the topographic layout of numerous biological features of the brain.