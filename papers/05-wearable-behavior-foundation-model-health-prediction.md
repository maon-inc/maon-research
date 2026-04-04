---
title: "Beyond Sensor Data: Foundation Models of Behavioral Data from Wearables Improve Health Predictions"
authors: "Erturk E et al."
year: 2025
journal: "arXiv (ICML 2025 Poster)"
doi: "arXiv:2507.00191"
url: "https://arxiv.org/abs/2507.00191"
domains: [5, 7]
relevance: 9
tags: ["foundation-model", "Apple-Watch", "behavioral-data", "health-prediction", "wearable", "sleep", "activity", "machine-learning", "digital-phenotyping"]
---

## Summary

Apple researchers developed the Wearable Behavior Model (WBM), a foundation model trained on behavioral signals from over 2.5 billion hours of Apple Watch data across 162,000 individuals in the Apple Heart and Movement Study. Unlike prior approaches that focus on raw sensor streams, WBM encodes higher-level behavioral patterns such as movement, sleep, and activity over time, then evaluates these representations across 57 health-related tasks.

## Key Findings

- WBM outperformed a strong PPG-based model in 18 of 47 static health prediction tasks and in nearly all dynamic (time-varying) prediction tasks
- The model excels in behavior-driven tasks such as sleep prediction, where daily patterns carry the most signal
- Combining WBM representations with raw sensor representations yields further improvements, demonstrating complementary information
- A systematic architecture and tokenization search was conducted to optimize for the unique properties of behavioral time series
- The model generalizes across diverse health outcomes including pregnancy detection (reported around 92% accuracy), cardiovascular risk, and mental health indicators
- The approach demonstrates that behavioral abstraction from wearables can be more informative than raw physiological data for many health outcomes

## MAON Applicability

Directly relevant to MAON's cognitive score feature, which already computes a composite health score from behavioral signals (steps, sleep, resting HR, HRV). This paper validates the principle that behavioral patterns from consumer wearables carry rich health information. MAON could consider similar multi-day behavioral pattern analysis rather than relying solely on single-day snapshots. The finding that behavior-level features outperform raw sensor features for many tasks supports MAON's approach of working with Apple Health summary metrics.

## Methodology Notes

Pre-training used over 2.5 billion hours of wearable data from 161,855 participants in the Apple Heart and Movement Study (AHMS). Evaluation covered 57 health-related tasks spanning both static classification and dynamic state prediction. Accepted as an ICML 2025 poster. The model uses a transformer architecture with custom tokenization strategies for behavioral time series.
