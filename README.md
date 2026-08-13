# Sleep, Stress, Anxiety and Personality Analysis

## Overview

This project investigates the relationships between sleep quality, daily stress, anxiety symptoms, chronotype, and BIS/BAS personality traits.

The analysis was performed using **jamovi** and includes descriptive statistics, normality testing, correlation analysis, and linear regression models.

---

## Dataset Variables

The dataset includes the following measures:

- **MEQ**: Morningness-Eveningness Questionnaire (chronotype)
- **STAI1**: Anxiety symptom measure
- **STAI2**: Anxiety symptom measure
- **Pittsburgh**: Sleep quality score
- **Daily_stress**: Daily stress level
- **BISBAS_bis**: Behavioral Inhibition System
- **BISBAS_reward**: Reward responsiveness
- **BISBAS_drive**: Goal drive
- **BISBAS_fun**: Fun seeking

Sample size:
- N = 22 participants
- MEQ had one missing value (N = 21)

---

## Statistical Analysis

The following analyses were conducted:

1. Descriptive statistics
   - Mean
   - Standard deviation
   - Minimum and maximum values

2. Normality assessment
   - Shapiro-Wilk test
   - Histograms
   - Q-Q plots

3. Correlation analysis
   - Pearson correlation
   - Spearman correlation

4. Linear regression analysis

---

## Main Findings

### Sleep Quality and Anxiety

**Pittsburgh → STAI1**

- R² = 0.312
- p = .007

Better/worse sleep quality showed a significant association with STAI1 anxiety symptoms.

---

### Personality Traits and Anxiety

**BISBAS_reward → STAI1**

- R² = 0.367
- p = .003

Reward responsiveness significantly predicted STAI1 anxiety symptoms.

---

**BISBAS_fun → STAI2**

- R² = 0.382
- p = .002

Fun seeking showed a significant association with STAI2 anxiety symptoms.

---

**BISBAS_bis → STAI2**

- R² = 0.207
- p = .033

Behavioral inhibition was significantly associated with STAI2 anxiety symptoms.

---

## Non-significant Findings

The following predictors did not show significant effects:

- MEQ → STAI1
- Pittsburgh → STAI2
- Daily_stress → STAI1
- BISBAS_drive → STAI1/STAI2

---

## Software

Analysis performed with:

- jamovi
- Version: [add your version if needed]

---

## Files

