---
title: "A machine-learning approach for stress detection using wearable sensors in free-living environments"
authors: "Various et al."
year: 2024
journal: "Computers in Biology and Medicine"
doi: "10.1016/j.compbiomed.2024.109035"
url: "https://www.sciencedirect.com/science/article/abs/pii/S0010482524010035"
domains: [3, 1]
relevance: 9
tags: ["machine-learning", "stress-detection", "wearable", "free-living", "heart-rate", "hrv", "ambulatory"]
---

## Summary

Develops and evaluates machine learning models for stress detection using wearable sensor data in free-living (non-laboratory) environments. Addresses the critical gap between lab-trained models and real-world deployment.

## Key Findings

- ML models trained on wearable sensor data can detect stress in free-living environments
- Heart rate and HRV features are among the most predictive features for stress classification
- Free-living stress detection is significantly more challenging than laboratory-based detection
- Personalized models (trained on individual baselines) outperform population-level models
- Multi-modal sensor fusion improves detection accuracy over single-signal approaches

## MAON Applicability

Directly relevant to MAON's stress detection model. Validates the personalized z-score approach MAON uses (comparing to individual baselines). The finding that real-world detection requires different approaches than lab settings informs MAON's ambulatory algorithm design.

## Methodology Notes

Published in Computers in Biology and Medicine (2024). Uses wearable sensors in free-living environments rather than lab settings. Tests multiple ML approaches. Addresses ecological validity of stress detection.
