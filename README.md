# Sleep, Stress, Anxiety and Personality Analysis

## Overview

This project investigates the relationships between sleep quality, daily stress, anxiety symptoms, chronotype, and BIS/BAS personality traits.

The analysis was performed using **jamovi** and includes descriptive statistics, normality assessment, correlation analysis, and linear regression models.

This study is an **exploratory analysis** due to the relatively small sample size.

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

### Sample Size

- Total participants: N = 22
- MEQ included one missing value (N = 21)

---

## Statistical Analysis

All analyses were conducted using **jamovi**.

The following analyses were performed:

### Descriptive Statistics

- Mean
- Median
- Standard deviation
- Minimum and maximum values

### Normality Assessment

Normality was assessed using:

- Shapiro-Wilk test
- Histograms
- Q-Q plots

Because some variables showed deviations from normality, both Pearson and Spearman correlations were examined.

### Correlation Analysis

- Pearson correlation
- Spearman correlation

### Linear Regression Analysis

Simple linear regression models were used to examine associations between sleep, stress, personality traits, and anxiety symptoms.

---

# Main Findings

## Sleep Quality and Anxiety

### Pittsburgh → STAI1

- R² = 0.312
- p = .007

Sleep quality was significantly associated with STAI1 anxiety symptoms.

---

# Personality Traits and Anxiety

## BISBAS_reward → STAI1

- R² = 0.367
- p = .003

Reward responsiveness showed a significant association with STAI1 anxiety symptoms.

---

## BISBAS_fun → STAI2

- R² = 0.382
- p = .002

Fun seeking showed a significant association with STAI2 anxiety symptoms.

---

## BISBAS_bis → STAI2

- R² = 0.207
- p = .033

Behavioral inhibition showed a significant association with STAI2 anxiety symptoms.

---

# Non-significant Findings

The following models did not show statistically significant associations:

- MEQ → STAI1
- Pittsburgh → STAI2
- Daily_stress → STAI1
- BISBAS_drive → STAI1
- BISBAS_drive → STAI2
- BISBAS_reward → STAI2

---

# Limitations

This study used a relatively small sample size (N = 22).

Therefore, findings should be interpreted as exploratory associations and should be confirmed in larger samples.

---

# Software

Analysis performed with:

- jamovi

---

# Repository Files

The repository contains:
