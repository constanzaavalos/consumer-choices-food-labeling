# Food Labeling: An Experiment to Assess Consumer Choices
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

The scope of this repository is to provide the comprehensive dataset and R analysis code utilized to determine the extent to which the presence or absence of different food labelling affects consumers' decision-making in an online shopping scenario.

Conceptually, the methodological approach and models can be split into the following components within the R Markdown document:
1. **Data Cleaning and Variable Recoding**
2. **Descriptive Statistics and Chi-Square Comparisons**
3. **ANOVA Comparisons (Treatment Groups vs. Outcomes)**
4. **Working Memory Test Metrics (hit rates, false alarms, and d' calculations)**
5. **Data Visualization (Boxplots, Distributions)**

## Repository Structure

The current version of the published package contains three primary files:
- `Food-labeling.-An-experiment-to-assess-consumer-choices  + Interactions number of calories 29112024 v6 trial specification Zvalues V2.Rmd`: The primary reproducible script containing all the data processing and statistical analysis.
- `Food_labelling_synthetic.csv`: The experimental dataset (collected August 2024) detailing participants' cereal choices and household circumstances.
- `s41043-025-01076-x.pdf`: The final published academic paper.

## Setup R Environment

Before running the analysis, please configure your `R` environment to ensure all script dependencies are met.

### Installing Dependencies

Open your standard R console or RStudio and run:

```r
install.packages(c("readr", "dplyr", "Matrix", "lme4", "texreg", "ggplot2", "tidyr"))
```

## Steps for running the analysis

1. Clone this GitHub repository locally.
```bash
git clone https://github.com/constanzaavalos/<Repository_Name>
cd <Repository_Name>
```

2. Open the `.Rmd` file in RStudio or your preferred IDE.
3. Update the working directory path in the `data` chunk to point to your local cloned repository directory (where `Food_labelling_synthetic.csv` is located).
4. Run all chunks sequentially or "Knit" the document to an HTML/PDF output to reproduce the full analysis results.
