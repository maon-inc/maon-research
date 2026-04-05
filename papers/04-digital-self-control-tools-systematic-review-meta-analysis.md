---
title: "Achieving Digital Wellbeing Through Digital Self-Control Tools: A Systematic Review and Meta-Analysis"
authors: "Lyngs U et al."
year: 2023
journal: "ACM Transactions on Computer-Human Interaction"
doi: "10.1145/3571810"
url: "https://dl.acm.org/doi/full/10.1145/3571810"
domains: [4]
relevance: 9
tags: ["digital-self-control", "screen-time", "meta-analysis", "systematic-review", "app-blocking", "intervention", "digital-wellbeing", "smartphone", "behavior-change"]
---

## Summary

A systematic review and meta-analysis evaluating the effectiveness of digital self-control tools (DSCTs) -- apps and features designed to help users manage their digital device usage. The meta-analysis found that DSCTs have a small to medium effect on reducing time spent on distractive technology, but effectiveness varies considerably based on intervention type and implementation approach.

## Key Findings

- Digital self-control tools produce a small to medium overall effect on reducing time spent on distractive technological sources
- Environmental modification interventions (blocking, restricting access) tend to be more effective than purely informational or awareness-based approaches
- Many studies do not examine compensatory behavior, where users shift screen time to other apps or devices rather than reducing total usage
- Personalization of interventions with respect to individual needs and lifestyles may be critical for sustained effectiveness
- Stand-alone interventions reduced target app usage by approximately 21% and helped individuals achieve self-defined goals for short durations
- Group-based and social accountability approaches showed promise for sustained behavior change, suggesting that community features can amplify individual interventions

## MAON Applicability

Directly relevant to MAON's smart schedule feature, which implements automated app blocking as a digital self-control intervention. The meta-analytic finding that environmental modification (blocking/restricting) outperforms awareness-only approaches validates MAON's architectural choice to use DeviceActivityMonitor-based blocking rather than simple usage tracking. The finding about compensatory behavior suggests MAON should monitor total screen time across categories, not just blocked apps. The personalization finding aligns with MAON's AI-driven approach to generating individualized blocking schedules.

## Methodology Notes

Systematic review and meta-analysis following PRISMA guidelines. Covers multiple randomized controlled trials and quasi-experimental studies of digital self-control tools. Analyzes both objective (device-measured) and subjective (self-reported) outcomes. Published in ACM Transactions on Computer-Human Interaction (2023).
