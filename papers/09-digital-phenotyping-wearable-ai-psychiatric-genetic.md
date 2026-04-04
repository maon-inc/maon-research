---
title: "Digital Phenotyping from Wearables Using AI Characterizes Psychiatric Disorders and Identifies Genetic Associations"
authors: "Liu JJ et al."
year: 2025
journal: "Cell"
doi: "10.1016/j.cell.2024.11.012"
url: "https://www.cell.com/cell/fulltext/S0092-8674(24)01329-1"
domains: [9, 4]
relevance: 9
tags: ["ADHD", "digital-phenotyping", "wearable", "actigraphy", "AI", "genetic-associations", "psychiatric-disorders", "adolescents", "ABCD-study", "machine-learning"]
---

## Summary

This Cell paper analyzed wearable and genetic data from the Adolescent Brain Cognitive Development (ABCD) study using an interpretable AI framework. The researchers derived over 250 wearable features as digital phenotypes to classify adolescents with psychiatric disorders (including ADHD and anxiety) and then used these features in genome-wide association studies (GWAS) to identify novel genetic loci linked to psychiatric conditions.

## Key Findings

- Machine learning models using solely objective wearable measures achieved high accuracy in classifying ADHD (AUC = 0.844)
- Models integrating both subjective and objective measures showed enhanced performance (AUC = 0.933)
- ADHD medication status classification reached AUC = 1.000 using objective measures alone
- The study identified 16 significant genetic loci and 37 psychiatric-associated genes, including ELFN1 and ADORA3
- Continuous wearable-derived features provided greater detection power than traditional case-control GWAS approaches
- The work demonstrates that wearable data can bridge phenotypic and genotypic characterization of psychiatric disorders

## MAON Applicability

Highly relevant to MAON's potential for detecting and supporting users with ADHD. The study validates that consumer-grade actigraphy data (similar to what MAON collects via Apple Health) contains meaningful signals for psychiatric classification. The 250+ feature set derived from wearable data could inform MAON's cognitive score algorithm, particularly for activity pattern analysis and sleep regularity metrics that distinguish ADHD profiles.

## Methodology Notes

Data from the ABCD study, a large longitudinal cohort of U.S. adolescents. Wearable data came from Fitbit devices worn by participants. Published in Cell (impact factor >60), one of the highest-impact journals. The interpretable AI framework allows feature importance analysis rather than relying on black-box models.
