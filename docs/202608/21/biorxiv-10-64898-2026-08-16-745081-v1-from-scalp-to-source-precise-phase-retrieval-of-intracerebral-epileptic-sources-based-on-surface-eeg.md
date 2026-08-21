---
title: "From Scalp to Source: Precise Phase Retrieval of Intracerebral Epileptic Sources Based on Surface EEG"
title_zh: 从头皮到源头：基于表面脑电的脑内癫痫源精确相位恢复
authors: "Furuglyas, K., Huszar-Kis, M., Horvath, B., Pejin, A., Forgo, N., Lango, I., Singla, S., Gorog, M., Vass, P., Chadaide, Z., Laszlovszky, T., Devinsky, O., Bagic, A. I., Somogyvari, Z., Berenyi, A."
date: 2026-08-20
pdf: "https://www.biorxiv.org/content/10.64898/2026.08.16.745081v1.full.pdf"
tags: ["query:eeg-priors"]
score: 8.0
evidence: EEG源定位，MRI引导逆解，偶极子估计
tldr: 深脑振荡相位追踪对闭环神经调控至关重要，但有创颅内记录在临床上受限，需无创方案。本文验证GN偶极子估计法，它无需解剖成像、计算高效，通过偶极子建模、降维及频率相关相位延迟校正从头皮EEG重建深脑源相位。在尸体重放与同步头皮-SEEG患者数据中，GN相位精度与信号保真度媲美MRI-informed逆解，尸体重建相关超过0.91且平均相位误差低于9度，患者相关约0.8。该方法为癫痫等疾病的相位锁定与闭环刺激提供低门槛、可扩展的无创通路。
source: biorxiv
selection_source: fresh_fetch
motivation: 深脑振荡相位追踪对闭环神经调控重要，但有创记录受限，急需无创高精度相位重建方法。
method: 验证GN偶极子估计法，采用偶极子建模、降维和频率相关相位延迟校正流水线，无需解剖成像。
result: 尸体数据中相位相关超过0.91且误差小于9度，患者数据中相关约0.8，与逆解相当。
conclusion: GN提供无创、低门槛的癫痫相位追踪方案，可促进相位锁定闭环刺激应用。
---

## 摘要
深部脑活动的精确相位追踪对于有效的闭环和锁相神经调控疗法至关重要。然而，由于侵入性，通过颅内记录直接获取深部神经相位在临床上仍受到限制。在此，我们验证并临床基准测试了Gabor-Nelson（GN）偶极子估计方法，用于从无创头皮脑电重建深部脑振荡相位。GN是一种基于几何、不依赖成像的方法，提供计算高效的偶极子重建，且很少被应用于人类神经科学中的源级相位估计。我们将GN与一种成熟的基于MRI的逆解（IS）方法进行了比较，采用包含偶极子建模、降维和频率相关相位延迟校正的三阶段重建流程。验证使用（i）尸体记录，其中已知的真实癫痫波形通过植入的深部电极回放，以及（ii）人类患者的同步头皮脑电和立体脑电记录，其中伪真实值通过颅内触点近似获得。在两个数据集中，GN达到了与IS相当的相位精度和信号保真度，尽管无需解剖成像。在尸体记录中，相位校正重建相关性超过r > 0.91，平均相位误差{Delta}{Phi} < 9度。在患者SEEG数据中，GN达到r约0.80，相位偏移适合神经调控时序。GN为传统逆建模提供了一种可行、低门槛、不依赖成像的替代方案，用于无创癫痫相位追踪。该框架为癫痫及可能其他基于网络的脑部疾病的可扩展锁相和闭环刺激疗法开辟了途径。

## Abstract
Accurate phase tracking of deep-brain activity is critical for effective closed-loop and phase-locked neuromodulation therapies. However, direct access to deep neural phase through intracranial recordings remains clinically restrictive due to the invasiveness. Here we validate and clinically benchmark the Gabor-Nelson (GN) dipole estimation method for reconstructing deep-brain oscillatory phase from non-invasive scalp EEG. GN is a geometry-based, imaging-independent approach that offers computationally efficient dipole reconstruction and has rarely been applied to source-level phase estimation in human neuroscience. We compared GN with an established MRI-informed Inverse Solution (IS) method using a three-stage reconstruction pipeline consisting of dipole modeling, dimensionality reduction, and frequency-dependent phase-delay correction. Validation is performed using (i) cadaveric recordings, where known ground-truth seizure waveforms were replayed through implanted deep electrodes, and (ii) simultaneous scalp EEG and SEEG recordings in human patients, where pseudo-ground truth was approximated via the intracranial contacts. GN achieved phase accuracy and signal fidelity comparable to IS across both datasets despite requiring no anatomical imaging. In cadaver recordings, phase-corrected reconstruction correlations exceeded r > 0.91 and {Delta}{Phi} < 9{degrees} in mean phase error. In patient SEEG data, GN reached up to r {approx} 0.80 with phase offsets suitable for neuromodulatory timing. GN offers a viable, low-barrier, imaging-independent alternative to traditional inverse modeling for non-invasive seizure phase tracking. This framework opens pathways for scalable, phase-locked and closed-loop stimulation therapies in epilepsy and potentially other network-based brain disorders.

---

## 论文详细总结（自动生成）

## 1. 核心问题与整体含义

- **研究动机**：深部脑振荡的相位信息对于闭环和锁相神经调控（如癫痫的闭环刺激）至关重要。然而，直接获取深部脑区相位通常依赖颅内记录（如SEEG），其侵入性限制了临床适用性和可扩展性。因此，需要一种无创、高精度、低门槛的深部源相位重建方法。
- **核心问题**：能否仅凭无创头皮EEG，可靠地恢复脑内癫痫源的振荡相位？现有方法如MRI-informed源逆解（IS）依赖个体解剖成像且计算成本高，难以广泛部署。本文探索并验证一种几何驱动的、不依赖成像的偶极子重建方法——Gabor-Nelson（GN），用于无创深部源相位追踪。
- **整体含义**：该研究为癫痫等神经疾病的闭环神经调控提供了可行的无创方案，有望降低技术门槛、扩大临床应用，并为基于网络的其他脑部疾病研究铺路。

## 2. 方法论

- **核心思想**：GN偶极子估计法基于头皮电极与脑内偶极子之间的几何关系，不依赖个体MRI或头模型，直接重建深部源的振荡相位。
- **技术流程**：采用三阶段重建流水线：
  1. **偶极子建模**：假设每个深部源可由一个或多个等效偶极子表示，基于电极位置和头皮几何计算正向传播矩阵。
  2. **降维**：对头皮EEG信号和偶极子空间进行降维处理，提高数值稳定性和计算效率，估计多个深部源的时域活动。
  3. **频率相关相位延迟校正**：由于容积传导和头皮-皮层距离引起的相位延迟，在频域上对重建相位进行校正，以匹配真实深部源的振荡时序。
- **对比方法**：与成熟且依赖MRI的逆解（IS）方法进行同样流程的对照，评估GN在无解剖成像前提下的相位重建性能。

## 3. 实验设计

- **数据集/场景**：
  1. **尸体记录**：在尸体上植入深部电极并回放已知的真实癫痫波形，作为ground truth，评估无创头皮EEG重建的准确度。
  2. **人类患者数据**：同时记录患者的头皮EEG和立体脑电（SEEG），以颅内触点信号作为伪ground truth，验证真实临床条件下的相位重建效果。
- **Benchmark**：以颅内记录（真值或伪真值）为金标准，衡量重建信号的相位一致性（相关系数r）和平均相位误差（ΔΦ）。
- **对比方法**：主要对比GN与MRI-informed逆解（IS）方法，两者采用相同的重建流程，仅有是否使用解剖成像的差异。

## 4. 资源与算力

- 原文摘要和元数据中**未明确报告**使用的GPU型号、数量、训练时长或具体算力配置。仅说明GN方法“计算高效”，可能暗示其算力需求低，但具体数值未披露。

## 5. 实验数量与充分性

- **实验数量**：摘要中提及两个独立数据集（尸体和患者），每个数据集估计包含多个记录通道或样本，但未给出具体的试验次数、患者人数或通道数量。未提及消融实验或参数敏感性分析。
- **充分性评估**：
  - 从验证维度看，同时包含已知真值（尸体）和临床近似真值（患者SEEG），增加了结论的可信度。
  - 但缺少对方法在不同癫痫类型、不同深部脑区、不同电极配置下的系统性测试；也未见与更多基线方法（如波束形成器、sLORETA）的对比，因此实验覆盖相对有限。
  - 未报告统计显著性检验或置信区间，公平性需进一步确认。

## 6. 主要结论与发现

- GN在无解剖成像的前提下，达到了与MRI-informed IS方法相当的相位精度和信号保真度。
- 尸体数据中，相位校正后重建相关超过r > 0.91，平均相位误差ΔΦ < 9度；患者SEEG数据中相关最高约0.80，相位偏移足以用于神经调控时序。
- 说明GN是一种可行、低门槛、不依赖成像的无创癫痫源相位追踪方法，可促进相位锁定和闭环刺激疗法的开发。

## 7. 优点

- **高创新性**：将GN偶极子估计方法引入人类神经科学中的源级相位估计，拓展了无创脑电分析工具。
- **实用性强**：无需MRI等解剖成像，简化了临床流程，降低设备与计算成本，适合广泛部署。
- **验证严谨**：使用尸体数据提供真实ground truth，并在临床患者中验证，兼顾内外部效度。
- **结果量化清晰**：给出明确的相关系数和相位误差指标，便于与其他方法比较。

## 8. 不足与局限

- **信息不完整**：论文预印本仅提供摘要，细节如具体算法公式、电极数量、患者人口学特征、数据预处理步骤等尚未公开，难以完全评估方法复现性。
- **实验覆盖有限**：仅针对癫痫数据，未涉及其他脑网络疾病；样本量未知，可能影响统计功效。
- **偏差风险**：患者SEEG的伪真值本身存在空间采样偏差，且头皮EEG和SEEG同步记录可能受信号泄漏干扰；尸体环境的电导特性与活体人类存在差异，可能高估或低估真实性能。
- **方法适用范围未明确**：GN基于几何假设，可能对深部源位置、颅骨各向异性、电极位置误差敏感，这些因素未在文中详细探讨。
- **缺乏算力报告**：未说明运行时间或资源需求，无法量化“计算高效”的具体程度。
- **对比方法数量单一**：仅与一种MRI-informed IS方法对比，缺少与当前主流无创源重建方法（如波束成形、稀疏源成像）的全面基准测试。

（完）
