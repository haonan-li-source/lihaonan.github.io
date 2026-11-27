---
layout: default
title: Personal Credit Default Risk Modeling
---

[← Portfolio](../../)

# Personal Credit Default Risk Modeling

<div class="project-meta"><strong>Role:</strong> Independent researcher, sole author, and corresponding author &nbsp; · &nbsp; <strong>Scale:</strong> 150,000 records</div>

<div class="project-actions"><a class="button" href="https://github.com/haonan-li-source/personal-credit-default-risk-modeling">View GitHub repository</a><a class="button" href="https://doi.org/10.1051/itmconf/20258001016">Read published paper</a></div>

## Research question

Only 6.68% of records in the study were defaults, so accuracy alone could hide poor detection of high-risk borrowers. I compared five classifiers on a common test set and examined how model choice changed ranking performance, minority-class recall, precision, and F1.

## Study design

- Used approximately 150,000 borrower records with ten credit features.
- Treated missing values and outliers and standardized relevant variables.
- Split training, validation, and test data before resampling.
- Applied SMOTE only to training data to prevent evaluation leakage.
- Compared logistic regression, decision tree, random forest, XGBoost, and LightGBM.
- Evaluated ROC-AUC, recall, precision, F1, and feature importance together.

## Key results

- Random forest achieved the highest ROC-AUC at 0.8391 and recall of 0.6858.
- LightGBM achieved precision of 0.2685 and F1 of 0.3557.
- LightGBM's F1 was approximately 54% higher than the logistic-regression result.
- Revolving credit utilization, number of dependents, and prior delinquency behavior were among the most informative factors.

## Challenge and solution

Improving default detection can also increase the number of lower-risk borrowers incorrectly flagged. I addressed this by keeping resampling inside the training set and interpreting recall, precision, F1, and ROC-AUC as a joint risk-management trade-off rather than selecting a model from one score.

## Publication

Published in *ITM Web of Conferences*, volume 80 (2025), article 01016. [Read the paper via DOI 10.1051/itmconf/20258001016](https://doi.org/10.1051/itmconf/20258001016).

## Outputs

Published paper, model-comparison tables, feature-importance interpretation, preprocessing and evaluation workflow, metric definitions, and citation information.

<div class="tag-list"><span>Credit Risk</span><span>Imbalanced Learning</span><span>Model Comparison</span><span>LightGBM</span><span>Financial Analytics</span></div>
