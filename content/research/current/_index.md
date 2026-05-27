+++
date = '2026-05-18T13:59:31+05:30'
draft = false
title = 'Current Research'
+++

## Beyond Convex Hull (BCH) Localization
<p align="center">
  <img src="/images/Dimension_Adatpation.png" width="500">
</p>

Conventional localization systems are typically designed assuming that the target lies inside the convex hull formed by the anchors. However, many emerging vehicular and UAV localization scenarios violate this assumption, since the targets are often located far outside the anchor region. In [1], [2], we have developed a mathematical framework to characterize the geometric limits of Time-of-Arrival (ToA)-based localization in such beyond convex hull scenarios. A key contribution was the derivation of a closed-form asymptotic scaling law showing that the ToA Dilution of Precision (DOP) increases linearly with the target distance for far-away targets. Using these insights, we've introduced the notion of Range-Normalized DOP (RNDOP) and formulated robust anchor placement strategies that minimize the worst-case positioning error for far-away targets [2]. Since the resulting optimization problem is highly non-convex under practical deployment constraints, we have developed iterative heuristic algorithms with different performance-complexity tradeoffs for robust anchor placement in vehicular and UAV systems. These frameworks provide practical design tools for localization systems employing vehicle-mounted or aerial anchors, and establish fundamental limits on achievable positioning accuracy in next-generation wireless localization networks.

Currently, we are 
1. extending our analysis of such scenarios to other techniques such as Time Difference of Arrival (TDoA), and incorporating measurement bias and heteroscedastic measurement errors, and
2. focusing on empirical validation of our theoretical results, and developing an richer understanding of localization error performance for BCH targets at intermediate distances. 

#### References
1. R. M. Rao, A. V. Padaki, B. L. Ng, Y. Yi, M. Kang, and V. Marojevic, “ToA-Based Localization of Far-Away Targets: Equi-DOP Surfaces, Asymptotic Bounds, and Dimension Adaptation,” IEEE Transactions on Vehicular Technology, vol. 70, no. 10, pp. 11089–11094, Oct. 2021.
2. R. M. Rao and D. R. Emenonye, “Iterative RNDOP-Optimal Anchor Placement for Beyond Convex Hull ToA-Based Localization: Performance Bounds and Heuristic Algorithms,” IEEE Transactions on Vehicular Technology, vol. 73, no. 5, pp. 7287–7303, May 2024.


## Integrated Sensing and Communications

<p align="center">
  <img src="/images/PO_PD.png" width="600">
</p>

Integrated sensing and communications (ISAC) is expected to become an important capability in future 6G wireless systems, where the same OFDM waveform simultaneously supports wireless communication and environmental sensing. In [1], we investigated monostatic OFDM-ISAC architectures under realistic hardware impairments such as residual self-interference, phase noise, and fractional-delay leakage. A key contribution of this work was identifying a fundamental limitation of conventional pilot-only sensing frameworks, where sparse pilot patterns generate deterministic ambiguity replicas in the range-Doppler map, resulting in ghost targets and elevated false-alarm rates in multi-target sensing scenarios. To address this, we proposed a data-aided sensing framework that exploits the full transmitted OFDM waveform—including both pilot and data-bearing symbols—to construct a denser sensing reference. This significantly suppresses pilot-induced ambiguities, improves coherent integration gain, and yields substantially better multi-target detection performance under realistic OFDM-ISAC operating conditions.

Currently, we are

1. extending these frameworks to long-range and high-velocity radar sensing using practical 5G NR waveforms, including targets operating beyond conventional cyclic-prefix-limited sensing regimes, and
2. developing low-complexity range-Doppler processing algorithms and SDR-based experimental testbeds to characterize the performance limits of data-aided sensing under realistic clutter, mobility, and hardware impairment conditions.

References

1. F. Faisal, R. M. Rao, A. S. Abdalla, and V. Marojevic, “Data-Aided Multi-Target Sensing for Monostatic OFDM-ISAC Systems with Hardware Impairments,” Under Review.