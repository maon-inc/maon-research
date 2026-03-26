---
title: "Exploring the Potential of Lightweight Large Language Models for AI-Based Mental Health Counselling Task: A Novel Comparative Study"
authors: "Maurya R et al."
year: 2025
journal: "Scientific Reports"
doi: "10.1038/s41598-025-05012-1"
url: "https://www.nature.com/articles/s41598-025-05012-1"
domains: [4]
relevance: 8
tags: ["LLM", "open-source", "lightweight", "mental-health", "chatbot", "BART", "T5", "FLAN-T5", "GODEL", "fine-tuning", "counselling"]
---

## Summary

A comparative evaluation of four lightweight open-source language models fine-tuned for automated mental health counseling: Google's T5-small, BART-base, FLAN-T5-small, and Microsoft's GODEL-base. The study demonstrates that smaller, resource-efficient models can generate empathetic and emotionally supportive mental health responses, with BART-base outperforming the others across all evaluation metrics.

## Key Findings

- BART-base achieved the best performance across all metrics: ROUGE-1 (0.4727), ROUGE-2 (0.2665), ROUGE-L (0.3554), and BLEU (25.3993)
- Lightweight models can run on consumer-grade hardware, making them viable for privacy-preserving on-device deployment
- BART-base generated responses that were rated as empathetic and emotionally supportive in qualitative assessment
- Fine-tuning on domain-specific mental health counseling data significantly improved response quality over base models
- T5-small and FLAN-T5-small showed competitive performance despite having fewer parameters
- The study highlights the tradeoff between model size, inference speed, and response quality for mental health applications

## MAON Applicability

Relevant to MAON's recent switch from Kimi K2.5 to GPT OSS 120B for AI operations. While MAON uses a larger model, this research validates the broader approach of using open-source/open-weight models for mental health conversational AI. The findings on fine-tuning strategies for empathetic response generation could inform how MAON's AI chat system is optimized. The privacy advantages of open-source models align with MAON's health data handling requirements, and the evaluation metrics provide benchmarks for assessing MAON's own chat quality.

## Methodology Notes

Comparative study using four pre-trained transformer models fine-tuned on mental health counseling datasets. Evaluation used automated metrics (ROUGE-1, ROUGE-2, ROUGE-L, BLEU) and perplexity scores. Models were fine-tuned with consistent hyperparameters to enable fair comparison. The study also included qualitative analysis of response characteristics including empathy, coherence, and clinical appropriateness.
