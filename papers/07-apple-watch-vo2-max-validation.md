---
title: "Investigating the Accuracy of Apple Watch VO2 Max Measurements: A Validation Study"
authors: "Lambe et al."
year: 2025
journal: "PLOS ONE"
doi: "10.1371/journal.pone.0323741"
url: "https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0323741"
domains: [7, 5]
relevance: 9
tags: ["apple-watch", "VO2-max", "validation", "cardiorespiratory-fitness", "wearable-accuracy", "consumer-device"]
---

## Summary

A validation study comparing Apple Watch VO2 max estimates against gold-standard maximal exercise treadmill testing using the modified Astrand protocol. Thirty participants wore an Apple Watch for 5 to 10 days to generate a VO2 max estimate, then completed laboratory testing. The Apple Watch systematically underestimated VO2 max, but the practical utility of passive daily estimation warrants further investigation.

## Key Findings

- Apple Watch underestimated VO2 max with a mean difference of 6.07 mL/kg/min (95% CI: 3.77 to 8.38)
- Mean absolute percentage error (MAPE) was 13.31% (95% CI: 10.01 to 16.61)
- Mean absolute error (MAE) was 6.92 mL/kg/min (95% CI: 4.89 to 8.94)
- Limits of agreement showed notable variability between methods (lower: -6.11, upper: 18.26 mL/kg/min)
- The Apple Watch consistently underestimated rather than overestimated, suggesting a directional bias
- Despite the bias, the passive and longitudinal nature of wrist-based estimation has practical advantages over lab testing

## MAON Applicability

MAON's baseline engine tracks VO2 max as a key vitals metric with a 30-day rolling window. This study helps calibrate expectations around Apple Watch VO2 max data flowing into the app. The systematic underestimation means MAON should interpret VO2 max trends (changes over time) rather than relying on absolute values for clinical-grade assessments. The 13% error rate is acceptable for trend detection and relative fitness tracking, which aligns with MAON's baseline comparison approach.

## Methodology Notes

Prospective validation study with 30 participants. Gold standard was maximal exercise treadmill test (modified Astrand protocol) with breath-by-breath gas analysis. Apple Watch worn for 5 to 10 days prior to lab testing. Bland-Altman analysis used for agreement assessment. Small sample limits generalizability across fitness levels and demographics.
