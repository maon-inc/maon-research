---
title: "Time2Stop: Adaptive and Explainable Human-AI Loop for Smartphone Overuse Intervention"
authors: "Chen M et al."
year: 2024
journal: "Proceedings of the CHI Conference on Human Factors in Computing Systems"
doi: "10.1145/3613904.3642747"
url: "https://pi.cs.tsinghua.edu.cn/wp-content/uploads/2024/05/chi24a-sub1586-cam-i16.pdf"
domains: [4, 3]
relevance: 10
tags: ["app-blocking", "screen-time", "JITAI", "context-aware", "machine-learning", "smartphone-overuse", "adaptive-intervention", "digital-wellbeing", "explainable-AI"]
---

## Summary

A CHI 2024 paper presenting Time2Stop, an adaptive and explainable human-AI system for smartphone overuse intervention. The system continuously gathers contextual and app usage data, transmits it to a cloud server for feature extraction and ML model inference, then generates personalized intervention prompts. Unlike static screen time limits, Time2Stop dynamically determines when to intervene based on the user's current context, achieving significantly higher acceptance rates than random prompting.

## Key Findings

- Context-aware intervention delivery achieved a 35% acceptance rate, nearly triple that of random prompts
- The ML model uses contextual features (time of day, location, app category, session duration) to predict optimal intervention timing
- Effectiveness varies by emotional state; "comforting" messages were more effective during stress, while "informational" messages worked better in neutral states
- Explainable AI components help users understand why an intervention was triggered, increasing trust and compliance
- The system adapts over time as it learns individual usage patterns and intervention receptivity
- Field deployment demonstrated feasibility of real-time context-aware digital wellbeing interventions

## MAON Applicability

Highly relevant to MAON's smart schedule and app blocking features. MAON currently implements context-aware blocking through calendar events (blocking during meetings) and server-driven schedules, but Time2Stop's approach of ML-driven intervention timing could enhance MAON's blocking strategy. The finding that intervention acceptance varies by emotional state supports MAON's integration of physiological stress signals (HRV) with screen time management. The explainability component aligns with MAON's AI summary and narrative features that help users understand their behavioral patterns.

## Methodology Notes

Full paper published at ACM CHI 2024 (top-tier HCI venue). Includes both system design and field deployment evaluation. The system was tested with real users in everyday settings, measuring intervention acceptance rates, screen time reduction, and user satisfaction. Comparison against random and rule-based intervention baselines demonstrates the advantage of adaptive, context-aware timing.
