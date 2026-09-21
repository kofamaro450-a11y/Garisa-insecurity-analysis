# Garisa-insecurity-analysis
Reproducible computational extension of my undergraduate thesis on Garissa County insecurity — adds quantitative and ML analysis on top of the original fieldwork, not a substitute for it.
# Garissa Insecurity: Research + Computational Extension

**This is not a repeat of the original research — it's an extension.** The
thesis (Layer A) is preserved exactly as researched. Everything else here is
a reproducible quantitative and machine-learning layer built *on top of* it.

*One research project from my portfolio, presented in two layers.*
Ziebi Kofa Maro · BA Political Science, The Catholic University of Eastern Africa

## Start here

**[`Garissa_Insecurity_Analysis.ipynb`](Garissa_Insecurity_Analysis.ipynb)** is
the single, self-contained entry point to this project — GitHub renders it
with every chart and result already embedded, so it opens fully formed with
no setup required. If you'd rather not open a notebook viewer, the identical
content is also in **[`Garissa_Insecurity_Analysis.html`](Garissa_Insecurity_Analysis.html)**
(download and open in any browser). Everything below the two-layer summary is
supporting detail for anyone who wants to dig into the code, the raw data, or
the original thesis directly.

## Key results at a glance

**Part 1 (real data):** the sample was 59% female, concentrated in the 36–50
age band (57.4%), with age distribution differing significantly by gender
(χ²(3, N=397) = 23.91, p < .001, Cramér's V = 0.245).

**Part 2 (synthetic-data ML demonstration):**

| Model | Accuracy | F1 | ROC-AUC |
|---|---|---|---|
| Baseline (majority class) | 0.58 | 0.00 | 0.50 |
| Logistic Regression | 0.60 | 0.50 | 0.64 |
| Decision Tree | 0.57 | 0.34 | 0.64 |
| Random Forest | 0.68 | 0.60 | 0.68 |

All three beat baseline; cross-validation shows the gap between them is not
statistically decisive at this sample size (297 training rows) — see the
notebook for the full, honest discussion of why that matters more than the leaderboard.

## Structure

### [Layer A — Original Empirical Research](layer-a-original-research/)

*Assessment of Kenya's Current Insecurity Challenges: A Case Study of Security
Challenges in Garissa County.* A genuine mixed-methods study: 397 survey
responses, 20 key-informant interviews, 4 focus group discussions, documented
sampling methodology, reliability testing, qualitative thematic analysis, and an
established conceptual framework. This establishes that the underlying research
is real, original social science — not a dataset picked off Kaggle. **This layer
is untouched by the extension below** — the original research stands on its own.

### [Layer B — Computational Social Science Extension](layer-b-computational-extension/)

This project extends my undergraduate research using reproducible quantitative
and machine-learning workflows. Because respondent-level data from the original
2023 fieldwork was not retained, the machine-learning component is presented as
a methodological demonstration using synthetic data and is not interpreted as
evidence about Garissa County.

Two parts:
1. A **reproducible rebuild of the thesis's real reported statistics**
   (descriptive figures + chi-square test), built from the actual numbers in
   Chapter Four.
2. A **synthetic-data ML pipeline demonstration** — preprocessing, feature
   engineering, a 75/25 train/test split, a majority-class baseline, three
   models (Logistic Regression, Decision Tree, Random Forest), 5-fold
   cross-validation, held-out evaluation (accuracy/precision/recall/F1/ROC-AUC),
   and interpretation of what each model learned. Full write-up and results
   table in [layer-b-computational-extension/README.md](layer-b-computational-extension/README.md).

## Why two layers, not one repeated study

Graduate admissions committees can tell the difference between "I ran a model on
a dataset" and "I designed and executed original research, then built a
reproducible technical layer on top of it." Keeping these separate — with an
explicit, honest boundary between real findings and a synthetic-data
demonstration — is the more credible story, not a weaker one.


leaderboard.

## Structure
