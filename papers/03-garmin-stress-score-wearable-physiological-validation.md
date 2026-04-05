---
title: "Assessing Stress Level Scores Against Wearables-Driven Physiological Measurements"
authors: "Rosenbach C et al."
year: 2025
journal: "Stress and Health"
doi: "10.1002/smi.70125"
url: "https://onlinelibrary.wiley.com/doi/full/10.1002/smi.70125"
domains: [3, 1]
relevance: 9
tags: ["Garmin", "stress-score", "HRV", "wearable-validation", "heart-rate", "physiological-stress", "consumer-wearable", "Vivosmart"]
---

## Summary

A validation study assessing the Garmin Vivosmart 4 stress level score against heart rate and HRV measurements from ECG recordings via the Polar H10 chest strap. The study included a pilot (n=29) followed by a preregistered main study (n=60), comparing Garmin's proprietary stress score with gold-standard physiological measurements during rest and mental stress tasks.

## Key Findings

- Garmin's stress score, mean HR, SD2/SD1, and HF power all exhibited significant differences between stress and rest conditions
- Garmin's stress score correlated significantly with HR, RMSSD, and SD2/SD1 ratio, confirming it tracks autonomic activation
- Heart rate emerged as the only parameter significantly associated with self-reported stress, while the Garmin stress score showed only a marginal effect on perceived stress
- The Garmin stress score reliably tracks autonomic activation associated with stress tasks but does not clearly distinguish between stress-related and non-stress-related arousal
- Composite stress scores from consumer wearables rely on unpublished proprietary algorithms, limiting transparency and scientific reproducibility
- The study was preregistered with power calculations, representing a methodological improvement over many prior wearable validation studies

## MAON Applicability

Directly relevant to MAON's Garmin integration feature. The validation results inform how MAON should interpret Garmin-derived stress data in its data context builders and cognitive scoring system. The finding that Garmin stress scores track autonomic activation but poorly predict subjective stress suggests MAON should use these scores as physiological signal indicators rather than direct proxies for user-perceived stress. This supports MAON's multi-signal approach of combining wearable data with self-report and behavioral data.

## Methodology Notes

Two-phase design: pilot study (n=29) for feasibility and power analysis, followed by preregistered main study (n=60). Laboratory protocol with alternating rest and mental-stress-inducing tasks. Simultaneous data collection from Garmin Vivosmart 4 (wrist) and Polar H10 (chest strap ECG). Self-reported stress collected alongside physiological measurements.
