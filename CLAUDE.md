# Research Paper Discovery Agent — MAON Vector Database

## Your Mission

You are a research agent finding peer-reviewed scientific papers for MAON, an AI-powered wellness companion. These papers will be embedded into a vector database that MAON queries at inference time to ground its pattern recognition in real science.

Save each paper as an individual markdown file in the `papers/` directory (see output format below). Aim for 10-15 high-quality papers per domain, ~100-150 papers total.

---

## What MAON Is

MAON is a consumer wellness app (NOT a medical/diagnostic tool) that detects emotional and behavioral drift before it becomes a problem. It works through iMessage/SMS conversations powered by an LLM with tool-use access to user data.

### Signals MAON Collects

**Physiological (Apple HealthKit via Apple Watch):**
- Heart rate (HR) — ~100-200 samples/day at 5-10 min intervals
- Heart rate variability (HRV) — overnight SDNN, plus RMSSD, pNN50
- Sleep stages — awake, core/light, deep, REM durations
- Respiratory rate — sleep-only, one value per night
- Wrist temperature — sleep-only, one value per night
- Blood oxygen saturation (SpO2)
- Steps, active energy, exercise minutes
- Body measurements (weight, height, body fat)
- Nutrition intake (caffeine, water, macronutrients)
- Wellness symptoms (mood, fatigue, headache — user-reported via HealthKit)

**Behavioral:**
- Screen time by app category (social media, gaming, shopping, entertainment, productivity)
- App pickup frequency and notification patterns
- App-switching frequency (attention fragmentation signal)

**Contextual:**
- Google Calendar event density, meeting gaps, free/busy
- Coarse location patterns (neighborhood-level, not GPS)
- Time of day, day of week

### ML Models MAON Runs

- **Stress detection** — real-time probability (0-100) from HR windows + HRV features, using ONNX neural net or LightGBM. Features: HR mean/std/range/trend, HRV SDNN/RMSSD, hour-of-day. Personalized via z-scores against user baseline. Trained on the WESAD dataset.
- **Recovery score** — Pearson correlation-based, 0-100, using HRV + sleep quality + activity
- **Sleep quality** — MAE-based, 0-100, combining duration + architecture + physiology
- **Readiness** — multi-input combining stress + recovery + sleep
- **Illness detection** — anomaly detection (binary), using precision@k for imbalanced data
- **HRV trend analysis** — 7-day rolling mean/std, 14-day trend slope, 30-day z-score

### Conditions Users Self-Report During Onboarding

Depression, anxiety, ADHD, bipolar disorder, OCD, PTSD, eating disorders, stress/burnout, chronic pain, sleep disorders.

### How Papers Will Be Used

The vector DB will be queried when MAON's AI is:
- Interpreting a user's biosignal patterns (e.g., "HRV dropped 15% over 3 days — what does research say this correlates with?")
- Providing context-aware wellness suggestions grounded in evidence
- Understanding how a self-reported condition (e.g., ADHD) manifests in the wearable signals MAON has access to
- Deciding whether a pattern is meaningful enough to proactively reach out about

MAON does NOT diagnose. Papers are used to inform pattern recognition and wellness nudges, not clinical decisions.

---

## 10 Priority Search Domains

### Domain 1: HRV and Mental Health

**Why it matters to MAON:** HRV is MAON's richest single physiological signal. The app tracks overnight SDNN and computes RMSSD, pNN50, and 30-day z-scores. Papers here directly improve how MAON interprets HRV changes.

**Search for:**
- HRV as a biomarker for anxiety, depression, PTSD, emotional dysregulation
- Vagal tone and autonomic nervous system balance in mood disorders
- HRV biofeedback intervention effectiveness
- SDNN vs RMSSD vs pNN50 — which metrics best predict which states
- HRV thresholds that distinguish clinical from subclinical stress
- Polyvagal theory and practical wearable applications
- HRV changes preceding mood episodes (predictive value)

**Key search terms:** "heart rate variability depression," "HRV anxiety biomarker," "vagal tone mental health," "HRV PTSD wearable," "autonomic function mood disorders," "HRV emotional regulation"

---

### Domain 2: Sleep Architecture and Mood Disorders

**Why it matters to MAON:** MAON tracks full sleep staging (awake, light, deep, REM) nightly. Understanding how sleep architecture shifts relate to mood states lets MAON detect early warning signs.

**Search for:**
- REM sleep changes in depression (REM latency, REM density)
- Deep sleep deficits in anxiety disorders
- Sleep stage patterns preceding bipolar manic/depressive episodes
- Sleep fragmentation and next-day mood/cognitive function
- Sleep architecture in ADHD (delayed sleep phase, reduced deep sleep)
- Wearable-measured sleep vs polysomnography accuracy
- Sleep quality composite scores and mental health outcomes

**Key search terms:** "sleep architecture depression," "REM sleep mood disorders," "deep sleep anxiety," "sleep stages bipolar episode prediction," "wearable sleep staging accuracy," "sleep fragmentation cognitive function"

---

### Domain 3: Heart Rate Patterns and Stress/Burnout

**Why it matters to MAON:** MAON has continuous HR throughout the day and detects stress episodes from elevated HR relative to user baseline. Papers here refine what HR patterns actually mean.

**Search for:**
- Resting heart rate elevation as chronic stress marker
- Diurnal heart rate patterns and burnout
- Heart rate reactivity vs recovery — which better predicts stress outcomes
- HR during sleep as a recovery/stress indicator
- Occupational burnout detection via wearable HR
- HR response to cognitive/emotional stressors in ambulatory settings
- Correlation between HR trends and self-reported stress/mood

**Key search terms:** "resting heart rate stress," "heart rate burnout wearable," "diurnal heart rate pattern anxiety," "ambulatory heart rate stress detection," "heart rate recovery mental health," "nocturnal heart rate stress"

---

### Domain 4: Digital Behavior and Mental Health

**Why it matters to MAON:** MAON tracks screen time by app category, pickup frequency, and app-switching. This is the strongest real-time behavioral signal layer in the system.

**Search for:**
- Social media usage and depression/anxiety (dose-response, not just correlation)
- Passive consumption vs active use — differential mental health effects
- Phone pickup frequency as anxiety/stress biomarker
- App-switching and attention fragmentation
- Late-night screen use and sleep/mood next day
- Digital phenotyping — using phone usage patterns to predict mental health states
- Screen time interventions and wellbeing outcomes
- Problematic smartphone use scales and wearable correlates

**Key search terms:** "digital phenotyping mental health," "screen time depression dose response," "smartphone usage anxiety biomarker," "social media passive consumption mood," "phone pickup frequency stress," "app switching attention fragmentation," "late night screen use sleep"

---

### Domain 5: Wearable-Based Illness and Anomaly Detection

**Why it matters to MAON:** MAON runs an illness detection model using physiological anomalies. Papers here validate and improve the approach.

**Search for:**
- Consumer wearable detection of COVID-19, flu, infections (pre-symptomatic)
- Resting HR and HRV changes during illness onset
- Wrist temperature elevation as early illness signal
- Respiratory rate changes detectable by wearables during illness
- Multi-signal anomaly detection frameworks for health monitoring
- Apple Watch and Fitbit studies on illness detection accuracy
- Physiological recovery patterns post-illness via wearables

**Key search terms:** "wearable illness detection," "Apple Watch COVID detection," "Fitbit pre-symptomatic illness," "resting heart rate infection," "HRV illness onset," "wrist temperature fever wearable," "respiratory rate wearable infection"

---

### Domain 6: Circadian Rhythm Disruption

**Why it matters to MAON:** MAON sees late-night screen use, irregular sleep timing, and can correlate these with next-day biosignals. Circadian disruption is a key upstream cause of many conditions MAON's users report.

**Search for:**
- Social jetlag and mental health outcomes
- Irregular sleep-wake patterns and depression risk
- Blue light/screen exposure timing and circadian disruption
- Chronotype and mood disorder risk
- Circadian rhythm disruption in bipolar disorder
- Wearable-detected rest-activity rhythm regularity and health outcomes
- Melatonin suppression from evening screen use

**Key search terms:** "social jetlag depression," "irregular sleep timing mental health," "circadian disruption bipolar," "chronotype mood disorder," "rest-activity rhythm wearable," "evening screen blue light circadian," "sleep regularity index mental health"

---

### Domain 7: Activity, Sedentary Behavior, and Mental Health

**Why it matters to MAON:** MAON tracks steps, active energy, and exercise minutes. Understanding the dose-response relationship between movement and mood helps calibrate when low activity is a concern.

**Search for:**
- Exercise as intervention for depression (effect sizes, dose-response)
- Sedentary behavior independent risk for anxiety/depression
- Steps per day and mood outcomes (thresholds, diminishing returns)
- Movement patterns (not just total activity) as mental health indicators
- Physical activity and sleep quality bidirectional relationship
- Acute vs chronic exercise effects on HRV and stress reactivity
- Breaking up sedentary time — mental health benefits

**Key search terms:** "exercise depression meta-analysis," "sedentary behavior anxiety," "steps per day mood," "physical activity HRV," "movement patterns mental health wearable," "exercise dose response depression," "sedentary breaks wellbeing"

---

### Domain 8: Respiratory Rate and Autonomic Function

**Why it matters to MAON:** MAON collects nightly respiratory rate from Apple Watch. This is an underutilized signal that may carry meaningful information about anxiety, stress, and autonomic state.

**Search for:**
- Respiratory rate during sleep and anxiety disorders
- Breathing patterns as autonomic nervous system indicators
- Respiratory sinus arrhythmia (RSA) and emotional regulation
- Slow breathing interventions and anxiety/stress reduction
- Nocturnal respiratory rate trends and illness/stress detection
- Respiratory rate variability as complement to HRV
- Wearable respiratory rate accuracy and clinical utility

**Key search terms:** "respiratory rate anxiety sleep," "breathing pattern autonomic function," "respiratory sinus arrhythmia emotion," "nocturnal respiratory rate wearable," "respiratory rate variability stress," "slow breathing anxiety intervention"

---

### Domain 9: ADHD and Behavioral/Physiological Signals

**Why it matters to MAON:** ADHD is one of the most commonly self-reported conditions by MAON users. Understanding how ADHD manifests in the signals MAON collects (screen time patterns, HRV, sleep, activity) is critical.

**Search for:**
- ADHD and smartphone usage patterns (excessive use, app-switching, reward-seeking apps)
- HRV differences in ADHD (autonomic dysregulation)
- Sleep disturbances in ADHD (delayed phase, reduced deep sleep, fragmentation)
- ADHD and screen time — bidirectional relationship
- Digital phenotyping of ADHD symptoms via phone sensors
- Physical activity patterns in ADHD
- Emotional dysregulation in ADHD — physiological correlates

**Key search terms:** "ADHD smartphone usage patterns," "ADHD heart rate variability," "ADHD sleep architecture," "ADHD screen time," "ADHD digital phenotyping," "ADHD autonomic function," "ADHD emotional dysregulation physiological"

---

### Domain 10: Eating Disorders and Physiological Markers

**Why it matters to MAON:** MAON tracks HR, HRV, nutrition intake (caffeine, water, macros), body measurements, and activity. Users may self-report eating disorders. Understanding the physiological signatures helps MAON recognize concerning patterns.

**Search for:**
- Heart rate and HRV changes in anorexia, bulimia, binge eating disorder
- Bradycardia as marker of restrictive eating
- Overexercise detection via wearable activity patterns
- Nutritional intake patterns and mood/energy correlations
- Wearable detection of compensatory behaviors
- Recovery monitoring in eating disorders via physiological signals
- Night eating and circadian/metabolic disruption

**Key search terms:** "eating disorder heart rate wearable," "anorexia HRV bradycardia," "overexercise detection wearable," "binge eating physiological markers," "eating disorder recovery monitoring," "nutritional intake mood wearable," "night eating circadian"

---

## Paper Quality Filters

### Prefer
- Uses **consumer-grade wearables** (Apple Watch, Fitbit, Garmin, Oura) — not just clinical-grade ECG/EEG
- Provides **quantitative thresholds or ranges** (e.g., "HRV SDNN below 50ms associated with 2x depression risk")
- Studies **real-world/ambulatory** monitoring, not just lab settings
- **Meta-analyses and systematic reviews** are highest value
- **Validation studies** of wearable accuracy for specific metrics
- Papers referencing the **WESAD dataset** (used in MAON's stress model training)
- Large sample sizes (n > 50 for observational, n > 20 for interventional)
- Published in reputable journals (JMIR, Nature Digital Medicine, Sensors, Psychophysiology, etc.)

### Avoid
- Papers requiring **clinical-grade equipment only** (medical ECG, PSG, EEG) with no wearable applicability
- Pure **pharmacological studies** without biosignal components
- Papers **older than 2015** unless foundational/highly cited (>500 citations)
- **Animal studies**
- **Case reports** (n=1)
- Papers behind paywalls with no accessible abstract/summary containing useful data
- Opinion pieces, editorials, conference abstracts without full methodology

---

## Output Format

Save each paper as a separate markdown file in `papers/`. Use this exact format:

**Filename:** `papers/{domain-number}-{short-kebab-case-title}.md`
Example: `papers/01-hrv-depression-meta-analysis.md`

**File content:**

```markdown
---
title: "Full Paper Title Here"
authors: "First Author et al."
year: 2023
journal: "Journal Name"
doi: "10.xxxx/xxxxx"
url: "https://doi.org/10.xxxx/xxxxx or direct link"
domains: [1]
relevance: 9
tags: ["hrv", "depression", "meta-analysis", "wearable"]
---

## Summary

2-3 sentence summary of what the paper found and why it matters for MAON.

## Key Findings

- Finding 1 with specific numbers (e.g., "HRV SDNN was 23% lower in depressed vs control group, p < 0.001")
- Finding 2 with quantitative data
- Finding 3

## MAON Applicability

1-2 sentences on how MAON could use this information. Which signal does it inform? How would it change pattern interpretation?

## Methodology Notes

Brief note on study design, sample size, wearable used (if applicable), and any limitations worth noting.
```

**Field definitions:**
- `domains`: Array of domain numbers (1-10) this paper covers. Many papers span multiple domains.
- `relevance`: 1-10 score. 10 = directly validates a signal MAON collects with quantitative thresholds from consumer wearables. 1 = tangentially related.
- `tags`: Lowercase keywords for future search/filtering.

---

## Workflow Instructions

1. **Work domain by domain**, starting from Domain 1 through Domain 10
2. For each domain, use WebSearch to find papers. Try multiple search queries — use the suggested search terms as starting points but adapt based on what you find
3. For each promising paper, get enough detail to fill the output template (you may need to search for the specific paper to find its abstract/findings)
4. Save each paper immediately as a file in `papers/` — don't batch them up
5. Prioritize **breadth first** (cover all 10 domains) then **depth** (go back for more papers in high-yield domains)
6. If a paper spans multiple domains, list all relevant domain numbers in the `domains` field and file it under the primary domain number
7. Prefer open-access papers where the full text or at least a detailed abstract is available
8. When you find a highly relevant paper, check its references and "cited by" for related work
9. Track your progress — after finishing all domains, do a gap analysis and fill holes

**Target: 100-150 papers total, roughly 10-15 per domain.**
