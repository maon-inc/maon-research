---
title: "Building Trust in Mental Health Chatbots: Safety Metrics and LLM-Based Evaluation Tools"
authors: "Park et al."
year: 2024
journal: "arXiv (preprint)"
doi: "arXiv:2408.04650"
url: "https://arxiv.org/abs/2408.04650"
domains: [4]
relevance: 9
tags: ["LLM", "chatbot", "safety", "evaluation", "mental-health", "benchmark", "automated-assessment"]
---

## Summary

This paper presents an evaluation framework for assessing the safety and reliability of mental health chatbots powered by large language models. The authors developed 100 benchmark questions and five guideline criteria for chatbot responses, then explored automated evaluation methods including LLM-based scoring, an agentic approach using real-time data, and embedding models to compare chatbot responses against ground truth standards.

## Key Findings

- Developed a structured safety evaluation framework with 100 benchmark questions spanning diverse mental health scenarios
- Proposed five core guideline criteria for evaluating mental health chatbot responses: clinical accuracy, empathy, safety, boundary awareness, and referral appropriateness
- LLM-based automated scoring showed promising correlation with human expert evaluations, suggesting feasibility of scalable quality assessment
- The agentic evaluation approach using real-time data provided more nuanced assessment than static benchmarks alone
- Embedding-based comparison methods offered computationally efficient alternatives for continuous monitoring of chatbot output quality
- Highlighted that only 16% of LLM-based mental health chatbot studies have undergone clinical efficacy testing as of 2024

## MAON Applicability

Directly relevant to MAON's new DSPy prompt optimization pipeline and LLM-as-judge evaluation system. The safety metrics and automated evaluation approaches described can inform how MAON evaluates and validates its AI-driven chat responses via the Sendblue worker. The benchmark question methodology could serve as a template for MAON's own evaluation suite, and the safety criteria align with the app's proactive agent and conversation management features.

## Methodology Notes

The study used a multi-method evaluation approach combining expert-developed benchmarks with automated assessment tools. While published as a preprint, the work was conducted by a multidisciplinary team including nursing informatics, computer science, psychiatry, and psychology researchers. The framework was validated against responses from multiple commercial and research chatbot systems.
