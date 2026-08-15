# Sleep & Anxiety Analysis

An exploratory statistical analysis of sleep, stress, chronotype, personality-related measures, and anxiety using the **MMASH (Multilevel Monitoring of Activity and Sleep in Healthy People)** dataset.

---

## About This Project

This project presents an exploratory statistical analysis conducted using the **MMASH (Multilevel Monitoring of Activity and Sleep in Healthy People)** dataset.

The original MMASH dataset contains data collected from **22 healthy participants**. I used these existing data to investigate relationships between sleep characteristics, psychological factors, personality-related measures, and anxiety symptoms.

The dataset itself was obtained from PhysioNet and was not collected or created by me. My work in this project focuses on the **statistical analysis, interpretation, visualization, and reporting of the existing data**.

---

## Author

**Maryam Sh**

GitHub: [@MSH9898](https://github.com/MSH9898)

### My Contribution

I independently conducted the statistical analysis of the MMASH dataset, including:

- Selection of relevant variables
- Data preparation and organization
- Descriptive statistics
- Assessment of normality
- Pearson correlation analysis
- Spearman correlation analysis
- Simple linear regression analyses
- Interpretation of statistical results
- Data visualization
- Preparation of the statistical analysis report using jamovi

The original data were obtained from the MMASH dataset available through PhysioNet.

---

## Research Question

This exploratory analysis investigates whether sleep-related and psychological variables are statistically associated with anxiety symptoms.

The main analyses examined relationships between:

- Sleep quality and anxiety
- Daily stress and anxiety
- Chronotype and anxiety
- BIS/BAS personality measures and anxiety

---

## Dataset

### MMASH — Multilevel Monitoring of Activity and Sleep in Healthy People

The analysis was conducted using data from **22 healthy participants** included in the MMASH dataset.

The dataset contains measurements related to:

- Sleep
- Physical activity
- Heart rate
- Stress
- Anxiety
- Emotions
- Chronotype
- Personality characteristics
- Cortisol and melatonin

### Original Dataset

[PhysioNet — MMASH Dataset](https://physionet.org/content/mmash/1.0.0/)

The data belong to the original dataset authors. This repository does not claim ownership of the MMASH dataset.

This repository documents my own statistical analysis and interpretation of the publicly available MMASH data.

---

## Variables

The main variables included in the analysis were:

| Variable | Description |
|---|---|
| `STAI1` | State anxiety score |
| `STAI2` | Trait anxiety score |
| `Pittsburgh` | Sleep quality measure |
| `Daily_stress` | Daily stress measure |
| `MEQ` | Morningness-Eveningness Questionnaire score |
| `BISBAS_bis` | Behavioral Inhibition System score |
| `BISBAS_reward` | Reward responsiveness score |
| `BISBAS_drive` | Drive score |
| `BISBAS_fun` | Fun-seeking score |

---

## Methodology

The statistical analysis was performed using **jamovi (Version 2.7)**.

The analysis included:

1. Data inspection and preparation
2. Descriptive statistics
3. Shapiro-Wilk normality tests
4. Pearson correlation analysis
5. Spearman correlation analysis
6. Simple linear regression analyses
7. Data visualization
8. Interpretation of statistical findings

Because several variables showed deviations from normality, both Pearson and Spearman correlation analyses were examined.

---

## Descriptive Statistics

The dataset contained **22 participants**.

The MEQ variable contained one missing observation, resulting in **N = 21** for analyses involving MEQ. All other variables included in the descriptive analysis had N = 22. :contentReference[oaicite:2]{index=2}

| Variable | Mean | SD | Min | Max |
|---|---:|---:|---:|---:|
| MEQ | 50.2 | 6.52 | 38 | 64 |
| STAI1 | 36.0 | 9.35 | 24 | 59 |
| STAI2 | 39.4 | 10.3 | 0 | 49 |
| Pittsburgh | 7.50 | 8.60 | 3 | 45 |
| Daily stress | 32.2 | 17.1 | 2 | 74 |
| BIS | 22.5 | 2.50 | 19 | 26 |
| Reward | 20.1 | 2.39 | 17 | 25 |
| Drive | 12.3 | 1.96 | 8 | 16 |

---

## Normality Assessment

Normality was assessed using the **Shapiro-Wilk test**. :contentReference[oaicite:3]{index=3}

| Variable | Shapiro-Wilk p |
|---|---:|
| MEQ | .613 |
| STAI1 | .028 |
| STAI2 | < .001 |
| Pittsburgh | < .001 |
| Daily stress | .220 |
| BIS | .040 |
| Reward | .050 |
| Drive | .241 |

Several variables showed evidence of deviation from normality, particularly STAI1, STAI2, Pittsburgh, and BIS.

---

## Correlation Analysis

Pearson and Spearman correlations were examined between daily stress, anxiety scores, and sleep quality. :contentReference[oaicite:4]{index=4}

### Daily Stress and STAI1

Pearson correlation:

- **r = -0.155**
- **p = .490**

Spearman correlation:

- **rho = -0.020**
- **p = .929**

No statistically significant association was observed between daily stress and STAI1.

### Daily Stress and STAI2

Pearson correlation:

- **r = -0.426**
- **p = .048**

Spearman correlation:

- **rho = -0.175**
- **p = .436**

The Pearson correlation was statistically significant, while the Spearman correlation was not.

### STAI1 and STAI2

Pearson correlation:

- **r = 0.340**
- **p = .122**

Spearman correlation:

- **rho = 0.573**
- **p = .005**

The Spearman correlation indicated a statistically significant positive association between STAI1 and STAI2.

### Pittsburgh and STAI1

Pearson correlation:

- **r = 0.559**
- **p = .007**

Spearman correlation:

- **rho = 0.305**
- **p = .168**

The Pearson correlation indicated a statistically significant positive association between Pittsburgh and STAI1.

### Pittsburgh and STAI2

Pearson correlation:

- **r = 0.157**
- **p = .484**

Spearman correlation:

- **rho = 0.167**
- **p = .459**

No statistically significant association was observed between Pittsburgh and STAI2.

---

## Linear Regression Results

Simple linear regression models were used to examine associations between selected predictors and anxiety scores.

### Pittsburgh → STAI1

Sleep quality (`Pittsburgh`) significantly predicted STAI1:

- **R = 0.559**
- **R² = 0.312**
- **B = 0.608**
- **SE = 0.202**
- **t = 3.01**
- **p = .007**
- **N = 22**

The model explained approximately **31.2% of the variance** in STAI1. :contentReference[oaicite:5]{index=5}

---

### Daily Stress → STAI1

Daily stress was not a statistically significant predictor of STAI1:

- **R = 0.155**
- **R² = 0.0241**
- **B = -0.0848**
- **SE = 0.121**
- **t = -0.703**
- **p = .490**
- **N = 22**

The model explained approximately **2.4% of the variance** in STAI1. :contentReference[oaicite:6]{index=6}

---

### Daily Stress → STAI2

Daily stress significantly predicted STAI2 in the linear regression model:

- **R = 0.426**
- **R² = 0.182**
- **B = -0.256**
- **SE = 0.122**
- **t = -2.11**
- **p = .048**
- **N = 22**

The model explained approximately **18.2% of the variance** in STAI2. :contentReference[oaicite:7]{index=7}

---

### MEQ → STAI1

MEQ was not a statistically significant predictor of STAI1:

- **R = 0.00155**
- **R² = 2.41e-6**
- **B = -0.00191**
- **SE = 0.282**
- **t = -0.00676**
- **p = .995**
- **N = 21**

The model explained virtually none of the variance in STAI1. :contentReference[oaicite:8]{index=8}

---

## BIS/BAS Measures and STAI1

### BIS → STAI1

- **R = 0.411**
- **R² = 0.169**
- **B = 1.54**
- **p = .057**
- **N = 22**

The association did not reach the conventional statistical significance threshold of .05. :contentReference[oaicite:9]{index=9}

### Reward Responsiveness → STAI1

- **R = 0.606**
- **R² = 0.367**
- **B = 2.37**
- **SE = 0.697**
- **t = 3.403**
- **p = .003**
- **N = 22**

Reward responsiveness was a statistically significant predictor of STAI1 and the model explained approximately **36.7% of the variance**. :contentReference[oaicite:10]{index=10}

### Drive → STAI1

- **R = 0.359**
- **R² = 0.129**
- **B = 1.72**
- **p = .101**
- **N = 22**

Drive was not a statistically significant predictor of STAI1. :contentReference[oaicite:11]{index=11}

### Fun-Seeking → STAI1

- **R = 0.388**
- **R² = 0.151**
- **B = 1.18**
- **SE = 0.628**
- **t = 1.88**
- **p = .074**
- **N = 22**

Fun-seeking was **not** statistically significant as a predictor of STAI1 at the .05 level. :contentReference[oaicite:12]{index=12}

---

## BIS/BAS Measures and STAI2

### BIS → STAI2

- **R = 0.455**
- **R² = 0.207**
- **B = 1.87**
- **SE = 0.819**
- **t = 2.284**
- **p = .033**
- **N = 22**

BIS was a statistically significant predictor of STAI2. :contentReference[oaicite:13]{index=13}

### Reward Responsiveness → STAI2

- **R = 0.305**
- **R² = 0.0927**
- **B = 1.31**
- **p = .168**
- **N = 22**

Reward responsiveness was not a statistically significant predictor of STAI2. :contentReference[oaicite:14]{index=14}

### Drive → STAI2

- **R = 0.143**
- **R² = 0.0205**
- **B = 0.753**
- **p = .525**
- **N = 22**

Drive was not a statistically significant predictor of STAI2. :contentReference[oaicite:15]{index=15}

### Fun-Seeking → STAI2

- **R = 0.618**
- **R² = 0.382**
- **B = 2.07**
- **SE = 0.589**
- **t = 3.52**
- **p = .002**
- **N = 22**

Fun-seeking was a statistically significant predictor of STAI2 and the model explained approximately **38.2% of the variance**. :contentReference[oaicite:16]{index=16}

---

## Main Findings

The exploratory analysis identified several statistically significant associations within the sample.

The regression models with the largest R² values were:

- **Fun-seeking → STAI2:** R² = 0.382
- **Reward responsiveness → STAI1:** R² = 0.367
- **Pittsburgh → STAI1:** R² = 0.312
- **BIS → STAI2:** R² = 0.207
- **Daily stress → STAI2:** R² = 0.182

The strongest model was the association between **fun-seeking and STAI2**, which explained approximately **38.2% of the variance** in STAI2 in this sample.

The analysis also identified a statistically significant association between **Pittsburgh and STAI1**.

These findings represent **statistical associations within the analyzed sample** and should not be interpreted as evidence of causality.

---

## Limitations

Several limitations should be considered when interpreting the findings:

- The sample size is small (**N = 22**).
- The analysis is based on an existing dataset rather than newly collected data.
- The data are observational, so causal relationships cannot be established.
- Several variables showed deviations from normality.
- The MEQ analysis was based on **N = 21** because of one missing observation.
- Some Pearson and Spearman correlations produced different conclusions, highlighting the importance of considering distributional characteristics.
- Multiple statistical analyses were conducted, increasing the possibility of chance findings.
- The findings may not generalize to other populations.
- The results should therefore be considered **exploratory** and interpreted cautiously.

---

## Repository Contents

| File | Description |
|---|---|
| `sleep_anxiety_analysis.omv.omv` | Jamovi project containing the statistical analyses |
| `jamovi_result.pdf` | Exported statistical analysis results |
| `README.md` | Project documentation |

---

## Tools

- **jamovi 2.7** — Statistical analysis
- **R 4.5** — Statistical computing environment used by jamovi
- **GitHub** — Version control and project documentation
- **PhysioNet / MMASH** — Original data source

---

## Reproducibility

The statistical analyses can be reviewed in the included Jamovi project:

`sleep_anxiety_analysis.omv.omv`

The exported statistical results are available in:

`jamovi_result.pdf`

---

## Attribution

The MMASH dataset was obtained from PhysioNet:

[MMASH Dataset — PhysioNet](https://physionet.org/content/mmash/1.0.0/)

The original dataset and its authors are credited as the source of the data.

**This repository represents my own statistical analysis of the publicly available MMASH dataset, not my own data collection.**

---

## Project Status

**Status: Completed exploratory analysis**

