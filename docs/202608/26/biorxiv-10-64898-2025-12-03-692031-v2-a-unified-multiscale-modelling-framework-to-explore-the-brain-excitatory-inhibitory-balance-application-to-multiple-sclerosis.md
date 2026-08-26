---
title: "A unified multiscale modelling framework to explore the brain excitatory-inhibitory balance: application to multiple sclerosis"
title_zh: 探索大脑兴奋-抑制平衡的统一多尺度建模框架：应用于多发性硬化症
authors: "Korkmaz, G., Lorenzi, R. M., Ravera, F., Alahmadi, A. A. S., Monteverdi, A., Kanber, B., Prados, F., D'Angelo, E. U., Palesi, F., Toosy, A., Gandini Wheeler-Kingshott, C. A. M."
date: 2026-08-19
pdf: "https://www.biorxiv.org/content/10.64898/2025.12.03.692031v2.full.pdf"
tags: ["query:eeg-priors"]
score: 6.0
evidence: 结合DCM与TVB，利用结构和功能先验建模脑亚网络，可迁移用于EEG脑区先验。
tldr: 兴奋-抑制平衡是大脑网络正常运作的基础，其失衡与多发性硬化症（MS）等神经疾病密切相关。本研究结合动态因果建模（DCM）与虚拟大脑（TVB），构建统一多尺度框架，分析健康对照和MS患者的视觉运动网络任务态及静息态fMRI数据。结果显示MS患者整体网络架构虽保留，但特定连接（如小脑至初级视觉皮层）由抑制性转为兴奋性，任务态反馈连接异常，且与行为及临床指标相关。该框架将网络级兴奋性增益与连接级有效连接强度关联起来，为揭示脑疾病中兴奋-抑制失衡机制提供了新途径。
source: biorxiv
selection_source: fresh_fetch
motivation: 脑网络兴奋-抑制平衡紊乱与多发性硬化症相关，但现有模型难以跨尺度表征，故需统一框架。
method: 结合DCM与TVB，对任务和静息fMRI及扩散成像数据建模，分析视觉运动网络的有效连接与兴奋性增益。
result: MS患者网络架构保留，但小脑至V1连接由抑制转兴奋，任务态反馈连接为负且随负荷恶化，并与行为/临床相关。
conclusion: 集成DCM与TVB揭示全局兴奋性增益调节任务相关有效连接，提供理解MS兴奋-抑制失衡的多尺度框架。
---

## 摘要
兴奋与抑制的平衡对于大脑动力学至关重要，其破坏可导致神经系统疾病中的网络功能障碍。在此，我们提出一个概念上统一的脑多尺度建模框架，结合应用于任务态和静息态功能磁共振成像（fMRI）数据的动态因果建模（DCM）以及虚拟大脑（TVB），来表征大脑的兴奋/抑制平衡。我们将该框架应用于一个由9名健康对照者和17名多发性硬化症（pwMS）患者组成的队列中的视觉运动脑亚网络。采集的数据包括具有可变握力的事件相关任务fMRI实验、静息态fMRI和弥散加权成像。视觉运动网络包括双侧初级视觉皮层（V1）、左侧初级运动皮层（M1）、辅助运动区和前运动皮层（SMAPMC）、扣带皮层（CC）、顶上小叶（SPL）以及右侧小脑小叶VI（CR）。DCM结果显示，虽然MS中的整体网络结构得以保留，但有效连接的兴奋/抑制性质存在显著改变：在静息状态下，观察到CR到V1连接的统计变化，该连接在健康志愿者中为抑制性，而在MS中为兴奋性。在任务期间，有效连接反馈（包括小脑自连接）在健康志愿者中为正性，但在MS中为负性，并随着运动需求的增加而日益失调。功能和有效连接的改变与行为表现（任务反应时间）和临床测量（残疾严重程度）相关。在整体组水平上，TVB参数将NMDA介导的兴奋性增益降低与较慢的任务反应相关联。此外，整合DCM和TVB表明，更高的全局兴奋性增益与感觉运动和视觉运动通路中更强的任务参与有效连接相关，从而将TVB捕获的网络水平兴奋性与上下文依赖的定向交互重配置及DCM揭示的连接水平强度联系起来。

## Abstract
Balanced excitation and inhibition are essential for brain dynamics, and their disruption can lead to network dysfunction in neurological diseases. Here, we present a conceptually unified multiscale brain modelling framework combining Dynamic Causal Modelling (DCM) applied to task and resting-state functional Magnetic Resonance Imaging (fMRI) data and The Virtual Brain (TVB) to characterise the excitatory/inhibitory balance of the brain. We applied the framework to a visuomotor brain subnetwork in a cohort of 9 healthy controls and 17 people with multiple sclerosis (pwMS). Acquired data included an event-related task fMRI experiment with variable grip force, resting-state fMRI, and diffusion-weighted imaging. The visuomotor network comprised the bilateral primary visual cortex (V1), left primary motor cortex (M1), supplementary motor and premotor cortex (SMAPMC), cingulate cortex (CC), superior parietal lobule (SPL), and right cerebellar lobule VI (CR). Results from DCM showed that while the overall network architecture was preserved in MS, there were significant alterations in the excitatory/inhibitory nature of effective connectivity: at rest, a statistical change was observed in CR-to-V1 connectivity, which was inhibitory in healthy volunteers but excitatory in MS. During task, effective connectivity feedback, including cerebellar self-connection, was positive in healthy volunteers but negative in MS and became increasingly dysregulated with higher motor demand. Alterations in functional and effective connectivity were associated with behavioural performance (task reaction time) and clinical measures (disability severity). At the overall group level, TVB parameters linked reduced NMDA-mediated excitatory gain to slower task responses. Moreover, integrating DCM and TVB demonstrated that higher global excitatory gain was associated with stronger task-engaged effective connectivity across sensorimotor and visuomotor pathways, linking network-level excitability captured by TVB to context-dependent reconfiguration of directed interactions and to connection-level strength revealed by DCM.