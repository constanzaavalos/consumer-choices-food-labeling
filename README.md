# 🛒 Food Labeling: Consumer Choices Experiment

[![Language](https://img.shields.io/badge/Language-R-276DC3.svg)](https://www.r-project.org/)
[![Dataset](https://img.shields.io/badge/Dataset-Experimental-blue.svg)](#)
[![Models](https://img.shields.io/badge/Models-ANOVA_%7C_Ordinal_Logistic-lightgrey.svg)](#)
[![Status](https://img.shields.io/badge/Status-Published-success.svg)](#)

> **Executive Summary:** This repository provides the comprehensive dataset and reproducible R pipeline utilized to determine how the presence or absence of different physical food labels affects consumers' decision-making and working memory load during online grocery shopping.

## 🌍 Why This Matters
* **Consumer Protection:** Understanding how labels influence choices ensures better regulatory policies for public health and nutrition.
* **Cognitive Load:** The study evaluates not just *what* people choose, but how working memory acts as a hidden limiting factor in processing complex nutritional information.
* **Actionable Insights:** Provides statistical backing for the implementation of simplified, coarse vs. detailed nutritional labeling on packaging.

## 📊 Dataset
The exact variables and participant answers gathered in the study are provided cleanly in `Food_labelling_synthetic.csv`.
- **Source:** Online Experimental Survey (Collected August 2024)
- **Features:** Demographics, Cereal Choices (Absent, Coarse, Detailed Labels), Working Memory capacity (n-back tests).
- **Target Variable:** Consumer Preference and Nutritional Choice.

## 🔬 Methodology Pipeline

`Data Cleaning & Preprocessing` ➔ `Descriptive Statistics (Chi-Square)` ➔ `Treatment Group ANOVA` ➔ `Working Memory (d') Scoring` ➔ `Ordinal Logistic Modeling`

## 🤖 Models & Analysis Benchmarked
| Analytical Method | Purpose in Study |
| :--- | :--- |
| **Chi-Square Tests** | To verify demographic balance and independence across the three experimental treatment groups. |
| **ANOVA** | To determine statistically significant mean differences in cereal preferences across label constraints. |
| **Signal Detection Theory** | Calculating `d'` (d-prime) to measure cognitive sensitivity and distinction in the n-back memory tasks. |
| **Multilevel linear model and Multilevel logistic model** | Calculating `d'` (d-prime) to measure cognitive sensitivity and distinction in the n-back memory tasks. |

## 🚀 How to Run Locally

### 1. Prerequisites
Ensure you have **R or RStudio** installed with the following necessary libraries:
```R
install.packages(c("readr", "dplyr", "Matrix", "lme4", "texreg", "ggplot2", "tidyr"))
```

### 2. Execution
1. Clone the repository to your local machine.
2. Open `consumer_choices_analysis.Rmd` in RStudio.
3. Update the working directory path in the initial Data Import chunk to point to your cloned folder containing `Food_labelling_synthetic.csv`.
4. Run all chunks sequentially, or **Knit to HTML/PDF** to reproduce the entire study, outputs, and visualizations organically.

## 📁 Project Structure
The repository is kept intentionally flat for maximum reproducibility:
* `consumer_choices_analysis.Rmd` — The primary reproducible analysis pipeline.
* `Food_labelling_synthetic.csv` — The raw experimental dataset.

## 📄 Citation
If you use this code or dataset in your research, please cite the original paper:

> Avalos, C. (2025). Food label granularity and working memory: effects on food choice in a randomized controlled trial. *Journal of Health, Population and Nutrition*, *44*, Article 375. https://doi.org/10.1186/s41043-025-01076-x

---
👤 **Author**: Constanza Avalos-Valdebenito
