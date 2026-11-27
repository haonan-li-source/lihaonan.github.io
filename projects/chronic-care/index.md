---
layout: default
title: Chronic Care Pathway Risk Modeling
---

[← Portfolio](../../)

# Chronic Care Pathway Risk Modeling

<div class="project-meta"><strong>Role:</strong> Project lead and chief data analyst &nbsp; · &nbsp; <strong>Scale:</strong> 7.68M encounters &nbsp; · &nbsp; <strong>Focus:</strong> longitudinal risk modeling</div>

<div class="project-actions"><a class="button" href="https://github.com/haonan-li-source/chronic-care-pathway-risk-modeling">View repository and award evidence</a></div>

## Research question

Long gaps in care are often treated as empty intervals. This project tested whether an interruption longer than 90 days could instead serve as a useful signal of later acute care. It progressed from sequence-based patient segmentation to prediction of unplanned emergency or inpatient events after the first month of a disease-specific pathway.

## My contribution

I led data integration, encounter deduplication, pathway construction, feature design, clustering, predictive modeling, temporal validation, calibration, interpretation, and presentation. I also connected the original DataFest pathway insight with the later statistical-modeling framework, creating one coherent research progression.

## Methods

- Integrated seven de-identified EHR tables and resolved duplicate encounter identifiers.
- Encoded routine, specialist, and acute-care sequences, treating gaps longer than 90 days as explicit interruption signals.
- Used PCA and K-means to identify pathway patterns.
- Defined days 1–30 as the feature window and days 31–90 as the outcome window.
- Engineered utilization, disease-burden, pathway-entropy, and continuity features.
- Evaluated LightGBM with a logistic-regression reference, temporal splitting, bootstrap intervals, subgroup checks, Top-k capture, and Platt calibration.

## Key results

- Reconstructed 65,705 disease-specific pathways for 52,851 patients from approximately 7.68 million encounters.
- Identified an acutely unstable group representing 4.7% of patients; 59.2% of its post-interruption returns involved emergency or inpatient care.
- Achieved PR-AUC 0.187 against a 0.061 prevalence baseline and ROC-AUC 0.752.
- The highest-risk decile captured 33.7% of subsequent acute events.
- After Platt calibration, the Brier score was 0.054 versus a 0.058 event-rate baseline.
- A separate 180-day retrospective analysis found a 10.1% acute-event rate in the interrupted-follow-up group versus 1.0% in the stable-follow-up group.
- Received the 2026 ASA DataFest Best Insight Award and Beijing Division Second Prize in the 12th National College Student Statistical Modeling Competition.

## Challenge and solution

Low prevalence and longitudinal records can produce optimistic evaluation. I used calendar-based validation, fitted preprocessing only on the training period, separated feature and outcome windows, and reported PR-AUC, Top-k capture, and calibration alongside ROC-AUC. Duplicate encounter keys were resolved before pathway construction so repeated rows would not distort utilization features.

## Outputs

Competition papers, presentation decks, aggregate pathway figures, patient-segmentation summaries, risk-model evaluation tables, and outcome-window definitions.

<div class="tag-list"><span>Healthcare Analytics</span><span>Longitudinal Data</span><span>LightGBM</span><span>Risk Modeling</span><span>Calibration</span></div>
