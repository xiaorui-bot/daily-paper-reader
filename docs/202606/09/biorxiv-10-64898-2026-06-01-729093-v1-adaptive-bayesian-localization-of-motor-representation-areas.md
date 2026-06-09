---
title: Adaptive Bayesian localization of motor representation areas
title_zh: 运动表征区域的适应性贝叶斯定位
authors: "Laine, M., Mutanen, T. P., Parvin, S., Numssen, O., Weise, K., Stenroos, M., Granö, I., Soto, A. M., Matsuda, R. H., Souza, V. H., Knösche, T. R., Ilmoniemi, R. J."
date: 2026-06-04
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.01.729093v1.full.pdf"
tags: ["query:eeg-priors"]
score: 7.0
evidence: 自适应贝叶斯定位方法利用空间先验定位运动皮层
tldr: "传统经颅磁刺激定位运动皮层方法忽略空间信息或未利用先前反应。本文提出自适应贝叶斯定位法，实时优化电场并结合概率推理更新皮层起源分布，优化后续刺激。多线圈TMS实验表明，相较于随机定位，自适应法平均60次刺激即收敛，150次刺激后95%高密区常小于10 mm²，大幅减少所需刺激次数。"
source: biorxiv
selection_source: fresh_fetch
motivation: 减少TMS定位运动代表区域所需的刺激次数，提高临床效率。
method: 结合实时电场优化与贝叶斯概率更新，每刺激后更新皮层起源分布，优化后续刺激位置。
result: "自适应定位平均60次刺激收敛，刺激次数减半，95%高密区常小于10 mm²。"
conclusion: 自适应贝叶斯方法可高效、精准定位运动皮层，具临床潜力。
---

## 摘要
经颅磁刺激(TMS)能够非侵入性地定位皮层运动表征，在术前规划中具有重要的临床应用。现有方法要么忽略TMS诱导电场(E场)的空间信息，要么采用不利用先前诱发的运动反应来指导后续刺激的采集方案。我们提出了一种自适应贝叶斯定位方法，将实时E场优化与逐次试验的概率推断相结合。运动反应的皮层起源被表示为每次刺激后更新的空间概率分布。随后，根据之前的反应优化后续刺激，以最大化预期的定位改进。我们通过实验验证了该方法，使用多位点TMS进行自适应定位，并以随机线圈放置的单线圈TMS作为非自适应参考。在八名受试者中，与随机方案相比，自适应方案至少将稳定定位所需的刺激次数减半，平均在60次刺激内收敛，到150次刺激时，95%的最高密度区域通常低于10平方毫米。

## Abstract
Transcranial magnetic stimulation (TMS) enables non-invasive localization of cortical motor representations, with important clinical applications in presurgical planning. Existing methods either disregard spatial information about the TMS-induced electric field (E-field) or use acquisition schemes that do not leverage previously elicited motor responses to guide subsequent stimulation. We present an adaptive Bayesian localization method that combines real-time E-field optimization with per-trial probabilistic inference. The cortical origin of the motor responses is represented as a spatial probability distribution that is updated after each stimulus. Subsequent stimuli are then optimized to maximize the expected localization improvement given previous responses. We validated the method experimentally, using multi-locus TMS for adaptive localization and single-coil TMS as a non-adaptive reference with randomized coil placements. Across eight subjects, the adaptive protocol at least halved the number of stimuli required for stable localization compared to the randomized protocol, converging in 60 stimuli on average, with 95% highest-density regions often below 10 mm2 by 150 stimuli.