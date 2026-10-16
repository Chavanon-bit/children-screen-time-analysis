# Children's Screen Time Analysis

An academic Data Mining project exploring associations between children's screen-time categories and demographic, health, lifestyle, and environmental factors.

**Course:** ITCS444 Data Mining — Mahidol University  
**Year:** 2026  
**Status:** Phase 1 completed (Exploration & Design); clustering is planned, not yet implemented.

## Research question

What health, lifestyle, and environmental patterns are associated with children's screen-time levels?

The analysis is exploratory: observed associations **do not establish causation**.

## Dataset

- **Source:** 2024 National Survey of Children's Health (NSCH), Topical Public Use Dataset, U.S. Census Bureau
- **Size:** 51,375 observations and 457 original variables
- **Population:** Children aged 0–17 years in the United States
- **Scope for Phase 1:** Selected and prepared 15 candidate variables for exploratory analysis

The original dataset is not included in this repository. Obtain the official 2024 NSCH Topical public-use data from the U.S. Census Bureau / NSCH data release, and consult its documentation for variable definitions and usage terms.

## My contributions

This is a **team project**. My primary responsibility was **Exploratory Data Analysis (EDA)**, including:

- Producing descriptive summaries, cross-tabulations, and visualizations of screen-time patterns
- Comparing screen-time categories across **age**, **interest and curiosity in learning**, and **household food situation**
- Reviewing and studying the preprocessing code written by my teammate, including missing-value handling and data preparation

**Credit:** My teammate primarily implemented data preprocessing. The notebook includes both team members' work; the entire notebook should not be interpreted as code I independently authored.

## Phase 1 work and findings

The notebook covers candidate-variable selection, preprocessing, descriptive statistics, row-percentage comparisons, and feature assessment.

Selected findings reported in Phase 1:

- The share in the **4-or-more-hours** screen-time category ranged from **1.2% at age 0** to **43.7% at age 17**.
- By household food situation, the same category represented **21.0%** of children in households that could always afford nutritious meals and **44.1%** of children in households that often could not afford enough food.
- Differences in screen-time distributions were also explored by reported interest and curiosity in learning.

These descriptive findings do **not** demonstrate that age, food situation, or curiosity causes a change in screen time. Some groups and survey-coded categories require careful interpretation.

## Repository contents

- [`Data_Mining_preprocessed_EDA.ipynb`](./Data_Mining_preprocessed_EDA.ipynb) — Jupyter Notebook with team preprocessing, EDA code, displayed tables, and plots
- `README.md` — Project context, contributions, findings, and reproducibility notes

## How to review or run the notebook

1. Open the notebook directly on GitHub to inspect the saved tables and charts **without running the code**.
2. To rerun locally, install **Python**, **Jupyter Notebook**, **pandas**, and **matplotlib**, along with a working environment able to read Stata `.dta` files.
3. Download the official **2024 NSCH Topical** dataset and place `nsch_2024e_topical.dta` alongside the notebook (or adjust the local path).
4. Open `Data_Mining_preprocessed_EDA.ipynb` in Jupyter and run the cells in order.

The notebook expects the file `nsch_2024e_topical.dta`; this repository intentionally does not redistribute the dataset. Results may depend on library versions and the particular public-use dataset release. No automated reproducibility test is provided.

## Planned next phase

Explore clustering of selected demographic, health, lifestyle, and environmental characteristics, then assess and interpret the resulting groups. The Phase 1 report proposed **Gower distance**, **hierarchical clustering**, and **silhouette analysis**; these are **planned methods**, not completed results.
