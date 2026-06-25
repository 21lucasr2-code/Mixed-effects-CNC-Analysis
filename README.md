# Mixed-Effects Analysis of CNC Surface Roughness

## Overview

This project presents an end-to-end statistical analysis of CNC turning surface roughness using **R** and **mixed-effects modeling**. The objective is to investigate how machining parameters influence surface roughness while accounting for repeated measurements through random effects.

The analysis demonstrates a reproducible statistical workflow, including model fitting, hypothesis testing, residual diagnostics, and data visualization.

---

## Objectives

- Evaluate the effects of **depth of cut (ap)**, **cutting speed (vc)**, and **feed rate (f)** on surface roughness (Ra).
- Account for repeated measurements using a mixed-effects model.
- Assess model assumptions through diagnostic analyses.
- Produce publication-quality tables and visualizations.

---

## Dataset

- **Source:** Kaggle CNC Turning Dataset
- **Response Variable:** Surface Roughness (Ra)
- **Predictor Variables:**
  - Depth of Cut (ap)
  - Cutting Speed (vc)
  - Feed Rate (f)

---

## Statistical Methods

- Exploratory Data Analysis (EDA)
- Mixed-Effects Linear Modeling (`nlme`)
- Type III ANOVA
- Residual Diagnostics
- Variance Assessment
- Model Performance Evaluation

---

## R Packages

- `car`
- `dplyr`
- `effectsize`
- `emmeans`
- `ggplot2`
- `IRdisplay`
- `kableExtra`
- `knitr`
- `lme4`
- `modelsummary`
- `nlme`
- `patchwork`

---

## Repository Structure

```text
mixed-effects-cnc-analysis/
├── notebooks/
│   └── cnc_surface_roughness_analysis.ipynb
├── figures/
│   ├── boxplots_by_factor.png
│   ├── qq_plot.png
├── report/
│   └── final_report.pdf
├── README.md
└── LICENSE
```

---

## Results

### Distribution of Surface Roughness

![Boxplots](figures/boxplots_by_factor.png)

### Normal Q-Q Plot

![Q-Q Plot](figures/qq_plot.png)

---

## Project Highlights

- Built a mixed-effects model to examine how depth of cut, cutting speed, and feed rate influence CNC surface roughness.
- Found that feed rate had the greatest impact on surface roughness and remained the only consistently significant machining parameter.
- Observed a smaller but statistically significant effect from depth of cut, while cutting speed and interaction effects were not significant within the range of the experiment.
- Diagnostic checks revealed non-constant variance, so the model was refined with a heteroscedastic variance structure based on feed rate.
- The final model provided a more reliable representation of the machining process and demonstrated a complete, reproducible statistical analysis workflow in R.

---

## Skills Demonstrated

- R Programming
- Statistical Modeling
- Mixed-Effects Models
- ANOVA
- Experimental Design
- Data Visualization
- Regression Diagnostics
- Technical Reporting
- Reproducible Research

---

## Author

**Lucas Russo**

Bachelor of Science in Mathematics

This project was completed as part of my statistics portfolio to demonstrate practical applications of statistical modeling and data analysis in manufacturing.
