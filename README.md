# ANOVA Analysis on PlantGrowth Dataset

This project performs a statistical analysis of the `PlantGrowth` dataset using R. The analysis is documented in the `mod_stat_anova.rmd` R Markdown notebook.

## Overview

The `PlantGrowth` dataset consists of results from an experiment to compare yields (as measured by dried weight of plants) obtained under a control and two different treatment conditions.

## Analysis Steps

The notebook `mod_stat_anova.rmd` follows these steps:

1.  **Descriptive Analysis:**
    *   Loading the `PlantGrowth` dataset.
    *   Exploring the data structure and summary statistics.
    *   Visualizing plant weights per group using boxplots (saved as `boxplot.png`).

2.  **Statistical Modeling (ANOVA):**
    *   Fitting an ANOVA model to compare weights across groups.
    *   Interpreting the model coefficients.

3.  **Model Validation:**
    *   **Normality of Residuals:** Using the Shapiro-Wilk test to verify if residuals are normally distributed ($p > 0.05$).
    *   **Homogeneity of Variances:** Using Bartlett's test to verify if variances are consistent across groups ($p > 0.05$).

4.  **Post-hoc Testing (Tukey's HSD):**
    *   Performing Tukey's Honestly Significant Difference test for multiple comparisons between groups.
    *   Finding that only the difference between `trt2` and `trt1` is statistically significant.

5.  **Linear Regression:**
    *   Fitting a linear regression model as an alternative perspective on the group differences.

## Files in this Project

*   `mod_stat_anova.rmd`: The R Markdown source file containing the code and analysis.
*   `mod_stat_anova.nb.html`: The rendered R Notebook output.
*   `boxplot.png`: A boxplot visualization of the weights by group.

## Requirements

The analysis uses the following R packages:
*   `dplyr`
*   `ggplot2`
