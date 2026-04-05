---
title: "The Relation Between Passively Collected GPS Mobility Metrics and Depressive Symptoms: Systematic Review and Meta-Analysis"
authors: "Terhorst Y et al."
year: 2024
journal: "Journal of Medical Internet Research"
doi: "10.2196/51875"
url: "https://www.jmir.org/2024/1/e51875"
domains: [4, 7]
relevance: 9
tags: ["GPS", "mobility", "depression", "passive-sensing", "smartphone", "location", "meta-analysis", "digital-phenotyping"]
---

## Summary

A systematic review and meta-analysis examining the relationship between passively collected GPS mobility metrics and depressive symptoms across 19 studies involving 2,930 participants. The review synthesizes both between-person and within-person correlations, revealing that several GPS-derived features show significant associations with depression severity.

## Key Findings

- Significant between-person correlations with depression were identified for total distance traveled, normalized entropy, location variance, entropy, number of location clusters, and homestay duration
- GPS and WiFi association logs were the most commonly used sensors for mobility tracking across included studies
- The mean participant age was 28.42 (SD=18.96) with 59.64% female participants, indicating a skew toward younger populations
- Within-person associations were less consistently reported than between-person differences, suggesting individual baselines matter for longitudinal monitoring
- All 19 studies followed exploratory observational designs; no study fully adhered to STROBE reporting guidelines
- Large-scale heterogeneous samples (N>5,000) showed substantially lower prediction accuracy (AUC=0.57) compared to homogeneous student samples (AUC=0.82), highlighting generalizability challenges

## MAON Applicability

Directly relevant to MAON's location tracking feature, which collects GPS data and uploads location events to the Core Worker. The identified mobility metrics (distance, entropy, homestay, location clusters) could inform MAON's data context builders and cognitive scoring system. The finding that within-person changes may be more clinically meaningful than between-person differences supports MAON's approach of tracking individual trends over time rather than comparing against population norms.

## Methodology Notes

Systematic review and meta-analysis following PRISMA guidelines. Searched multiple databases for studies using passively collected smartphone GPS data with validated depression measures. Included 19 studies (N=2,930). Quality assessment noted that no included study fully met STROBE reporting standards, and most samples were relatively small and demographically homogeneous.
