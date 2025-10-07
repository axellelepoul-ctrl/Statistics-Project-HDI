# Statistics-Project-HDI

This R Notebook provides a comprehensive workflow for analyzing MOOC data. It includes data preparation, descriptive statistics, statistical testing, regression modeling, and visualizations.

The analysis starts by importing CSV files, merging usage data with questionnaires, and adding an iteration identifier. Derived variables are then created, such as the total number of videos watched (Videos_visonnees), total quizzes completed (Quizz_faits), learner categories (Complete, Disengaging_learners, Auditing_learners, Bystander), and a binary certification variable (Certificat.bin).

Descriptive analyses include contingency tables for HDI by gender, missing data summaries, and percentage calculations for each learner category. Visualizations such as heatmaps, mosaic plots, histograms, scatterplots, and boxplots are generated to explore the data and identify patterns.

Statistical analyses involve t-tests, Mann-Whitney tests, Kruskal-Wallis tests, linear regression, ANOVA with eta-squared effect sizes, and logistic regression to examine factors affecting certification probability. For count data like videos watched, Poisson and negative binomial regressions are used to account for overdispersion. Diagnostic checks, including QQ plots and residual plots, are applied to ensure model assumptions are met.

The notebook also covers additional analyses like correlation matrices, variance inflation factor (VIF) calculations, and alternative ANOVA applications for other datasets. Forest plots are included to visualize odds ratios from logistic models.

Important notes:

- Factor variables (like Gender) must be properly defined before analysis.
- CSV file paths should be updated to match your system.
- Odds ratio calculations require numeric p-values; convert with as.numeric() if necessary.
- MOOC count data may not perfectly follow a Poisson distribution due to overdispersion or heterogeneous participant behavior.

Required R packages include dplyr, tidyr, ggplot2, vcd, DescTools, afex, MASS, car, and corrplot.
