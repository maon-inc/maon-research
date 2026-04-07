---
title: "Exploring Wearable-Based Detection of Compulsive Handwashing in a Non-Controlled Setting: A Case Study"
authors: "Authors from ACM ISWC 2025"
year: 2025
journal: "Proceedings of the 2025 ACM International Symposium on Wearable Computers (ISWC '25)"
doi: "10.1145/3715071.3750434"
url: "https://dl.acm.org/doi/10.1145/3715071.3750434"
domains: [9, 5]
relevance: 8
tags: ["ocd", "compulsive-behavior", "handwashing", "wearable", "smartwatch", "machine-learning", "behavior-detection", "psychiatric-monitoring"]
---

## Summary

A case study exploring the feasibility of using smartwatch motion and location data to detect compulsive handwashing in a psychiatric ward setting. Over 63 hours of data from one participant captured 41 labeled handwashing acts, with machine learning models achieving strong performance in both detecting handwashing events and distinguishing compulsive from routine washing.

## Key Findings

- A Random Forest classifier achieved an F1 score of 0.710 for detecting handwashing events from continuous wrist-worn sensor data
- An LSTM model demonstrated high specificity (0.995) and moderate sensitivity (0.606) for handwashing detection
- Binary classification between compulsive and routine handwashing achieved an impressive F1 score of 0.94
- The system combined smartwatch-based motion data with location data to improve detection accuracy in naturalistic settings
- Unique kinematic patterns (repetitive and inertial motion) distinguished compulsive handwashing from similar non-OCD behaviors
- The approach demonstrated feasibility in an uncontrolled psychiatric ward environment, not just a laboratory

## MAON Applicability

Relevant to MAON's potential for detecting and monitoring behavioral patterns associated with OCD and other conditions in domain 09. While MAON currently focuses on physiological signals, this study demonstrates that consumer wearable motion data can objectively quantify compulsive behaviors. This approach could extend to detecting other repetitive behaviors relevant to OCD, ADHD, or anxiety, and could inform future JITAI-based intervention triggers for behavioral conditions.

## Methodology Notes

Single-participant case study conducted in a psychiatric ward. Collected 63+ hours of data with 41 labeled handwashing events using a smartwatch. Published in ACM ISWC 2025 proceedings. Evaluated Random Forest and LSTM classifiers. Limitations include very small sample size (n=1) and controlled clinical environment.
