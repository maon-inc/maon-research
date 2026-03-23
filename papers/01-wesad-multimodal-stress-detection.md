---
title: "Introducing WESAD, a Multimodal Dataset for Wearable Stress and Affect Detection"
authors: "Schmidt et al."
year: 2018
journal: "Proceedings of the 20th ACM International Conference on Multimodal Interaction (ICMI)"
doi: "10.1145/3242969.3242985"
url: "https://dl.acm.org/doi/10.1145/3242969.3242985"
domains: [1, 3]
relevance: 10
tags: ["wesad", "stress-detection", "wearable", "dataset", "multimodal", "hrv", "eda", "empatica"]
---

## Summary

The foundational paper introducing the WESAD dataset, which MAON's stress detection model is trained on. It provides multimodal physiological and motion data from both wrist-worn (Empatica E4) and chest-worn devices across 15 subjects under baseline, stress (Trier Social Stress Test), and amusement conditions.

## Key Findings

- Wrist-worn device achieved 87.12% accuracy for three-class classification (baseline, stress, amusement)
- Chest-worn device achieved higher accuracy at 92.28% for the same classification
- Blood volume pulse, electrodermal activity, and temperature from wrist device were most informative features
- The Trier Social Stress Test successfully induced measurable physiological stress responses detectable by consumer-grade wrist sensors

## MAON Applicability

This is the training dataset for MAON's stress detection model. Understanding its design, limitations (15 subjects, lab setting, specific stressor type), and feature importances is essential for MAON to contextualize its stress probability scores and communicate confidence levels.

## Methodology Notes

Lab study with 15 participants (12 male, 3 female; mean age 27.5). Used Empatica E4 (wrist) and RespiBAN (chest). Stress induced via TSST. Three conditions: baseline, stress, amusement. Published at ICMI 2018. Highly cited (>1500 citations). Dataset publicly available.
