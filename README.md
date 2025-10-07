# Statistics-Project-HDI

Description

This R Notebook contains a complete analysis of MOOC data, including:

Data preparation and cleaning from CSV files.

Creation of derived variables (e.g., Videos_visonnees, Quizz_faits, Certificat.bin).

Descriptive analysis (tables, percentages, missing values heatmaps).

Statistical tests: chi-square, ANOVA, t-test, Mann-Whitney.

Modeling: linear regression, logistic regression, Poisson and negative binomial regression.

Visualizations: histograms, scatterplots, boxplots, mosaic plots, and forest plots.

Notebook Structure

Data Preparation

Reading CSV files with proper encoding.

Merging usages and questionnaire datasets.

Adding the iteration column.

Creating the combined dataset effec_global.

Derived Variables

Videos_visonnees: total number of videos watched.

Quizz_faits: total number of quizzes completed.

Learner categorization: Complete, Disengaging_learners, Auditing_learners, Bystander.

Binary variable for certification: Certificat.bin.

Descriptive Analysis

Contingency table for HDI × Gender.

Mosaic plot to visualize associations.

Heatmap of missing values.

Percentage of students per category and iteration.

Statistical Analyses

Non-parametric tests: t-test, Mann-Whitney, Kruskal-Wallis.

Simple and multiple linear regression for Videos_visonnees.

ANOVA and eta² calculation for effect size.

Logistic regression to evaluate the influence of variables on certification probability.

Poisson and negative binomial regression for videos watched.

Visualizations

Scatterplots with regression lines.

Boxplots by category.

Mosaic plots with color based on standardized residuals.

Forest plots of odds ratios.

Diagnostics

Residual normality checks (QQ plots).

Residuals vs. fitted plots for linear models.

Overdispersion handling using negative binomial models.

Additional Analyses

Correlations and heatmaps.

Variance Inflation Factor (VIF) calculation for linear models.

ANOVA and Poisson model adjustments for other datasets.

Required Packages

dplyr, tidyr, ggplot2, vcd, DescTools, afex, MASS, car, corrplot.

Important Notes

File paths for CSV files must be updated according to your system.

Factor variables (e.g., Gender) must be correctly defined before analysis.

Forest plots and odds ratio calculations assume numeric p-values. Convert with as.numeric() if errors occur.

Poisson distribution may not perfectly fit MOOC data due to overdispersion and heterogeneous participant behavior.

Execution Instructions

Run the chunks in order to ensure all variables are created properly.

Check for warnings or errors when reading CSV files (proper encoding required).

Logistic regression coefficients and p-values are automatically extracted and converted into odds ratios with confidence intervals.
