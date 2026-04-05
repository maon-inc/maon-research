---
title: "Extending Stress Detection Reproducibility to Consumer Wearable Sensors"
authors: "Binte Amin O et al."
year: 2025
journal: "IEEE EMBC 2025"
doi: "10.48550/arXiv.2505.05694"
url: "https://arxiv.org/abs/2505.05694"
domains: [3, 1]
relevance: 8
tags: ["stress-detection", "consumer-wearable", "Garmin", "Forerunner-55", "Polar-H10", "Empatica-E4", "reproducibility", "HRV", "machine-learning", "AUROC"]
---

## Summary

This study examines stress detection reproducibility across consumer and research-grade wearable sensors, comparing the Garmin Forerunner 55, Polar H10, Empatica E4, and Biopac MP160. The research addresses the critical gap that most wearable stress detection studies focus on a single dataset and rarely evaluate model reproducibility across devices, populations, or study conditions.

## Key Findings

- Garmin Forerunner 55 achieved the best mental arithmetic stress detection in LOSO with AUROC up to 0.961, comparable to research-grade Polar H10 (AUROC 0.954)
- Empatica E4 achieved AUROC 0.905 with HRV-only model and 0.953 with HRV+EDA combined model
- Consumer wearables can achieve stress detection performance on par with research-grade devices in controlled settings
- Cross-device reproducibility remains a challenge, with performance variations depending on device placement and sensor type
- HRV-based features were the strongest predictors of stress across all device types
- Results suggest consumer wearables are viable for real-world stress monitoring applications

## MAON Applicability

Directly relevant to MAON's Garmin integration and stress monitoring features. Validates that consumer-grade Garmin devices can detect stress with high accuracy, supporting MAON's use of Garmin stress scores and HRV data in its cognitive score and wellness assessments. The reproducibility findings inform how MAON should handle data from different wearable sources (Apple Watch vs. Garmin) in its multi-signal composite scoring system.

## Methodology Notes

Comparative study using four device types (Biopac MP160, Polar H10, Empatica E4, Garmin Forerunner 55) during laboratory stress protocols including mental arithmetic tasks. Used Leave-One-Subject-Out (LOSO) cross-validation. Accepted at IEEE EMBC 2025.
