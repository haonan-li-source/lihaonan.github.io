---
layout: default
title: Tucson Yelp Sentiment Analysis
description: Review-level sentiment analysis and anonymous customer profiling on a 2,000-review Tucson course subset.
---

[← Portfolio](../../)

# Tucson Yelp Review Sentiment and Customer Profiles

<div class="project-meta"><strong>Format:</strong> Two-person course consulting project &nbsp; · &nbsp; <strong>Sample:</strong> 2,000 reviews &nbsp; · &nbsp; <strong>Focus:</strong> text analysis and privacy-aware reporting</div>

<div class="project-actions"><a class="button" href="https://github.com/haonan-li-source/tucson-yelp-sentiment-analysis">View GitHub repository</a></div>

## Research question

This project examined how review language, star ratings, and engagement signals describe restaurant experiences in Tucson. The implementation focused on two questions: how review-level sentiment varies with ratings and time, and whether repeat reviewers form distinct anonymous customer profiles.

## Methods

- Scored review text with VADER and TextBlob.
- Summarized sentiment by star rating and month.
- Aggregated repeat reviewers in memory and clustered standardized rating, sentiment, and engagement features.
- Used silhouette analysis to assess the selected four-cluster solution.
- Compared an engagement-only rating model with the same model plus VADER sentiment using five-fold cross-validation.
- Published only aggregate tables, model metrics, and de-identified figures.

## Verified results

- Analyzed 2,000 reviews from the original Tucson course subset.
- Clustered 134 repeat reviewers with at least two reviews into four groups.
- The four-cluster solution had a silhouette score of 0.387.
- Mean cross-validated R² was 0.092 for engagement-only features and 0.370 after adding VADER sentiment, a descriptive difference of 0.278 on this subset.

## My contribution

This was a two-person project. The submitted contribution statement records approximately 40% of the code and 60% of the poster writing and layout as my work. I contributed to the analysis, result interpretation, visual communication, and final presentation.

## Challenge and solution

Review text and user identifiers are analytically useful but should not appear in public outputs. The workflow keeps both fields in memory for scoring and aggregation, then exports only summary statistics, anonymous clusters, metrics, and de-identified figures. Word clouds and quoted “top reviews” were excluded because they could reveal individual language.

## Reproducibility boundary

The source CSV is not redistributed because it contains review text and user identifiers and remains subject to Yelp’s terms. The code and aggregate outputs are reproducible with the same 2,000-row course subset; a newly sampled Tucson subset may produce different counts and model results.

<div class="tag-list"><span>Sentiment Analysis</span><span>VADER</span><span>TextBlob</span><span>Clustering</span><span>Privacy-aware Reporting</span></div>
